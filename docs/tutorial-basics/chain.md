---
sidebar_position: 1
---

# Chain

Represents a connection to a specific blockchain. Used to fetch chain specific data like blocks, transactions, balances and fees.

:::note
Check out the base class for every blockchain: [Chain](../packages/classes/chainify_client.Chain.md)
:::

## Usage


### EVM
```ts
import { providers } from 'ethers';
import { Client } from '@liquality/client';
import { EvmNetworks, EvmChainProvider } from '@liquality/evm';

const provider = new providers.StaticJsonRpcProvider(EvmNetworks.ganache.rpcUrl);
const chainProvider = new EvmChainProvider(EvmNetworks.ganache, provider);
const client = new Client(chainProvider);

const currentBlock = await client.chain.getBlockHeight();
console.log(currentBlock)
```

### BTC
```ts
import { Client } from '@liquality/client';
import { BitcoinNetworks, BitcoinEsploraApiProvider } from '@liquality/bitcoin';

const chainProvider = new BitcoinEsploraApiProvider({
  batchUrl: 'https://electrs-batch-testnet-api.liq-chainhub.net/',
  url: 'https://electrs-testnet-api.liq-chainhub.net/',
  network: BitcoinNetworks.bitcoin_testnet,
  numberOfBlockConfirmation: 2,
});
const client = new Client(chainProvider);

const currentBlock = await client.chain.getBlockHeight();
console.log(currentBlock)
```

