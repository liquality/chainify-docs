---
sidebar_position: 3
---

# Swap

Used to initiate, claim or refund atomic swap transactions.

:::note
Check out the base class for every blockchain: [Swap](../packages/classes/chainify_client.Swap.md)
:::

:::note
You need a wallet provider for the swaps to work properly. Check the [previous section](./wallet.md) to see how to create one 
::: 

## Usage


### EVM
```ts
import { sha256 } from '@chainify/utils';
import { Client } from '@liquality/client';
import { EvmSwapProvider } from '@liquality/evm';

const swapProvider = new EvmSwapProvider({
  contractAddress: '0x133713376F69C1A67d7f3594583349DFB53d8166',
});
const client = new Client(chainProvider, walletProvider, swapProvider);

const refundAddress = await client.wallet.getAddress();
const secret = await client.swap.generateSecret('secret');
const secretHash = sha256(secret);

const swapParams = {
    asset: { isNative: true }, // swaping ETH
    value: new BigNumber(100000000); 
    recipientAddress: '0xe862a41cef3bbcc6d85bff8b9c36801a6bc4453e';
    refundAddress,
    secretHash,
    expiration: Math.round(Date.now() / 1000) + 3600;
}
const transaction = await client.swap.initiateSwap(swapParams);
console.log(transaction)

const claimTx = await client.swap.claimSwap(swapParams, transaction.hash, secret);
console.log(claimTx)

const refundTx = await client.swap.refund(swapParams, transaction.hash);
console.log(refundTx)
```

### BTC
```ts
import { sha256 } from '@chainify/utils';
import { Client } from '@liquality/client';
import { BitcoinNetworks, BitcoinSwapEsploraProvider } from '@liquality/bitcoin';

const swapProvider = new BitcoinSwapEsploraProvider({
  network: BitcoinNetworks.bitcoin_testnet,
  scraperUrl: 'https://electrs-testnet-api.liq-chainhub.net/',
});

const chainProvider = new BitcoinEsploraApiProvider({
  batchUrl: 'https://electrs-batch-testnet-api.liq-chainhub.net/',
  url: 'https://electrs-testnet-api.liq-chainhub.net/',
  network: BitcoinNetworks.bitcoin_testnet,
  numberOfBlockConfirmation: 2,
});

const client = new Client(chainProvider, walletProvider, swapProvider);

const refundAddress = await client.wallet.getAddress();
const secret = await client.swap.generateSecret('secret');
const secretHash = sha256(secret);

const swapParams = {
    asset: null, // no need to pass asset for BTC
    value: new BigNumber(100000000); 
    recipientAddress: 'bcrt1qa558ru7wyls34j6tnedtkmhfjgazwsk4l3sgac';
    refundAddress,
    secretHash,
    expiration: Math.round(Date.now() / 1000) + 3600;
}

const transaction = await client.swap.initiateSwap(swapParams);
console.log(transaction)

// if swap is not expired and secret is revealed
const claimTx = await client.swap.claimSwap(swapParams, transaction.hash, secret);
console.log(claimTx)

// if swap has expired
const refundTx = await client.swap.refund(swapParams, transaction.hash);
console.log(refundTx)
```

