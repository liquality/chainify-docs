---
id: "chainify_evm.EvmNftProvider"
title: "Class: EvmNftProvider"
sidebar_label: "EvmNftProvider"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).EvmNftProvider

## Hierarchy

- `default`<`BaseProvider`, `Signer`\>

  ↳ **`EvmNftProvider`**

  ↳↳ [`CovalentNftProvider`](chainify_evm.CovalentNftProvider.md)

  ↳↳ [`MoralisNftProvider`](chainify_evm.MoralisNftProvider.md)

  ↳↳ [`OpenSeaNftProvider`](chainify_evm.OpenSeaNftProvider.md)

## Constructors

### constructor

• **new EvmNftProvider**(`walletProvider`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `walletProvider` | [`EvmBaseWalletProvider`](chainify_evm.EvmBaseWalletProvider.md)<`BaseProvider`, `Signer`\> |

#### Overrides

Nft&lt;BaseProvider, Signer\&gt;.constructor

#### Defined in

[evm/lib/nft/EvmNftProvider.ts:22](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/nft/EvmNftProvider.ts#L22)

## Properties

### cache

• `Protected` **cache**: `Record`<`string`, `NftInfo`\>

#### Defined in

[evm/lib/nft/EvmNftProvider.ts:20](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/nft/EvmNftProvider.ts#L20)

___

### schemas

• `Protected` **schemas**: `Record`<`string`, `NftContract`\>

#### Defined in

[evm/lib/nft/EvmNftProvider.ts:19](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/nft/EvmNftProvider.ts#L19)

___

### walletProvider

• `Protected` **walletProvider**: `default`<`BaseProvider`, `Signer`\>

#### Inherited from

Nft.walletProvider

#### Defined in

client/dist/lib/Nft.d.ts:4

## Methods

### approve

▸ **approve**(`contractAddress`, `operator`, `tokenID`, `fee?`): `Promise`<`Transaction`<`TransactionResponse`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `contractAddress` | `AddressType` |
| `operator` | `AddressType` |
| `tokenID` | `number` |
| `fee?` | `FeeType` |

#### Returns

`Promise`<`Transaction`<`TransactionResponse`\>\>

#### Overrides

Nft.approve

#### Defined in

[evm/lib/nft/EvmNftProvider.ts:100](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/nft/EvmNftProvider.ts#L100)

___

### approveAll

▸ **approveAll**(`contractAddress`, `operator`, `state`, `fee?`): `Promise`<`Transaction`<`TransactionResponse`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `contractAddress` | `AddressType` |
| `operator` | `AddressType` |
| `state` | `boolean` |
| `fee?` | `FeeType` |

#### Returns

`Promise`<`Transaction`<`TransactionResponse`\>\>

#### Overrides

Nft.approveAll

#### Defined in

[evm/lib/nft/EvmNftProvider.ts:138](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/nft/EvmNftProvider.ts#L138)

___

### balanceOf

▸ **balanceOf**(`contractAddress`, `owners`, `tokenIDs`): `Promise`<`BigNumber` \| `BigNumber`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `contractAddress` | `AddressType` |
| `owners` | `AddressType`[] |
| `tokenIDs` | `number`[] |

#### Returns

`Promise`<`BigNumber` \| `BigNumber`[]\>

#### Overrides

Nft.balanceOf

#### Defined in

[evm/lib/nft/EvmNftProvider.ts:73](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/nft/EvmNftProvider.ts#L73)

___

### fetch

▸ **fetch**(): `Promise`<`NFTAsset`[]\>

#### Returns

`Promise`<`NFTAsset`[]\>

#### Overrides

Nft.fetch

#### Defined in

[evm/lib/nft/EvmNftProvider.ts:149](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/nft/EvmNftProvider.ts#L149)

___

### getWallet

▸ **getWallet**(): `default`<`BaseProvider`, `Signer`\>

#### Returns

`default`<`BaseProvider`, `Signer`\>

#### Inherited from

Nft.getWallet

#### Defined in

client/dist/lib/Nft.d.ts:7

___

### isApprovedForAll

▸ **isApprovedForAll**(`contractAddress`, `operator`): `Promise`<`boolean`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `contractAddress` | `AddressType` |
| `operator` | `AddressType` |

#### Returns

`Promise`<`boolean`\>

#### Overrides

Nft.isApprovedForAll

#### Defined in

[evm/lib/nft/EvmNftProvider.ts:132](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/nft/EvmNftProvider.ts#L132)

___

### setWallet

▸ **setWallet**(`wallet`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `wallet` | `default`<`BaseProvider`, `Signer`\> |

#### Returns

`void`

#### Inherited from

Nft.setWallet

#### Defined in

client/dist/lib/Nft.d.ts:6

___

### transfer

▸ **transfer**(`contractAddress`, `receiver`, `tokenIDs`, `amounts?`, `data?`, `fee?`): `Promise`<`Transaction`<`TransactionResponse`\>\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `contractAddress` | `AddressType` | `undefined` |
| `receiver` | `AddressType` | `undefined` |
| `tokenIDs` | `string`[] | `undefined` |
| `amounts?` | `number`[] | `undefined` |
| `data` | `string` | `'0x'` |
| `fee?` | `FeeType` | `undefined` |

#### Returns

`Promise`<`Transaction`<`TransactionResponse`\>\>

#### Overrides

Nft.transfer

#### Defined in

[evm/lib/nft/EvmNftProvider.ts:31](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/nft/EvmNftProvider.ts#L31)
