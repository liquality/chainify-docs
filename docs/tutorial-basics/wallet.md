---
sidebar_position: 2
---

# Wallet

Used to perform all signing-based operations. 

:::caution
A ***seed phrase*** is required for the wallet instance to work properly. Make sure the seed phrase is ***never*** leaked and ***always*** consider ***security first***.
:::

:::note
Check out the base class for every blockchain: [Wallet](../packages/classes/chainify_client.Wallet.md)
:::

:::note
You need a chain provider for the wallet to work properly. Check the [previous section](./chain.md) to see how to create one 
::: 

## Usage


### EVM
```ts
import { providers } from 'ethers';
import { Client } from '@liquality/client';
import { EvmNetworks, EvmChainProvider } from '@liquality/evm';

const walletOptions = { derivationPath: `m/44'/60'/0'/0/0'`, mnemonic: 'piece effort bind that embrace enrich remind powder sudden patient legend group' };
const walletProvider = new EvmWalletProvider(walletOptions, chainProvider);
const client = new Client(chainProvider, walletProvider);

const from = await client.wallet.getAddress();
const signature = await client.wallet.signMessage('secret', from)
console.log(signature)
```

### BTC
```ts
import { Client } from '@liquality/client';
import { BitcoinNetworks, BitcoinHDWalletProvider } from '@liquality/bitcoin';

const network = BitcoinNetworks.bitcoin_testnet;
const walletOptions = {
  network,
  baseDerivationPath: `m/84'/${network.coinType}'/0'`,
  mnemonic: 'piece effort bind that embrace enrich remind powder sudden patient legend group',
};

// we consider that the chain provider is already available. 
// check the previous section how to create a chain provider
const walletProvider = new BitcoinHDWalletProvider(walletOptions, chainProvider);
const client = new Client(chainProvider, walletProvider);

const from = await client.wallet.getAddress();
const signature = await client.wallet.signMessage('secret', from)
console.log(signature)
```

