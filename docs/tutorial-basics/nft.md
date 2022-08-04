---
sidebar_position: 4
---

# NFT

A way to fetch, transfer & manage non-fungible tokens. ERC721 & ERC1155 supported.


## Usage

There are 3 different NFT providers available - Moralis, Covalent & OpenSea


### Moralis
```ts
import { Client } from '@liquality/client';
import { MoralisNftProvider } from '@liquality/evm';

// Fetch NFTs from Moralis
const moralis = new MoralisNftProvider(walletProvider, {
  url: "",
  apiKey: "",
  appId: "",
});
const client = new Client().connect(moralis);

const nfts = await client.nft.fetch();
console.log(nfts)

// Transfer
const transaction = await client.nft
  .transfer(
    "0xe10cd16070101ffe6b5bdd380c3c7f0e8fcec84d", // nft contract address
    "0x8072aC361d0ee237EFE0883198613d8d121Ee98d", // recipient
    ["1"], // token ids
    ["1"] // token amounts only applicable for ERC1155
  );

console.log(transaction)
```

### Covalent
```ts
import { Client } from '@liquality/client';
import { CovalentNftProvider } from '@liquality/evm';

// Fetch NFTs from Covalent
const covalent = new CovalentNftProvider(walletProvider, {
  url: "https://api.covalenthq.com/v1",
  apiKey: "",
});
const client = new Client().connect(covalent);

const nfts = await client.nft.fetch();
console.log(nfts)

// Transfer
const transaction = await client.nft
  .transfer(
    "0xe10cd16070101ffe6b5bdd380c3c7f0e8fcec84d", // nft contract address
    "0x8072aC361d0ee237EFE0883198613d8d121Ee98d", // recipient
    ["1"], // token ids
    ["1"] // token amounts only applicable for ERC1155
  );

console.log(transaction)
```


### OpenSea
```ts
import { Client } from '@liquality/client';
import { OpenSeaNftProvider } from '@liquality/evm';

// Fetch NFTs from OpenSea
const openSea = new OpenSeaNftProvider(walletProvider, {
  url: "https://rinkeby-api.opensea.io/api/v1/",
  apiKey: '',
});
const client = new Client().connect(openSea);

const nfts = await client.nft.fetch();
console.log(nfts)

// Transfer
const transaction = await client.nft
  .transfer(
    "0xe10cd16070101ffe6b5bdd380c3c7f0e8fcec84d", // nft contract address
    "0x8072aC361d0ee237EFE0883198613d8d121Ee98d", // recipient
    ["1"], // token ids
    ["1"] // token amounts only applicable for ERC1155
  );

console.log(transaction)
```
