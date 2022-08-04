---
id: "chainify_evm.CovalentNftProvider"
title: "Class: CovalentNftProvider"
sidebar_label: "CovalentNftProvider"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).CovalentNftProvider

## Hierarchy

- [`EvmNftProvider`](chainify_evm.EvmNftProvider.md)

  ↳ **`CovalentNftProvider`**

## Constructors

### constructor

• **new CovalentNftProvider**(`walletProvider`, `config`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `walletProvider` | [`EvmBaseWalletProvider`](chainify_evm.EvmBaseWalletProvider.md)<`BaseProvider`, `Signer`\> |
| `config` | [`NftProviderConfig`](../namespaces/chainify_evm.EvmTypes.md#nftproviderconfig) |

#### Overrides

[EvmNftProvider](chainify_evm.EvmNftProvider.md).[constructor](chainify_evm.EvmNftProvider.md#constructor)

#### Defined in

[evm/lib/nft/CovalentNftProvider.ts:12](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/nft/CovalentNftProvider.ts#L12)

## Properties

### cache

• `Protected` **cache**: `Record`<`string`, `NftInfo`\>

#### Inherited from

[EvmNftProvider](chainify_evm.EvmNftProvider.md).[cache](chainify_evm.EvmNftProvider.md#cache)

#### Defined in

[evm/lib/nft/EvmNftProvider.ts:20](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/nft/EvmNftProvider.ts#L20)

___

### schemas

• `Protected` **schemas**: `Record`<`string`, `NftContract`\>

#### Inherited from

[EvmNftProvider](chainify_evm.EvmNftProvider.md).[schemas](chainify_evm.EvmNftProvider.md#schemas)

#### Defined in

[evm/lib/nft/EvmNftProvider.ts:19](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/nft/EvmNftProvider.ts#L19)

___

### walletProvider

• `Protected` **walletProvider**: `default`<`BaseProvider`, `Signer`\>

#### Inherited from

[EvmNftProvider](chainify_evm.EvmNftProvider.md).[walletProvider](chainify_evm.EvmNftProvider.md#walletprovider)

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

#### Inherited from

[EvmNftProvider](chainify_evm.EvmNftProvider.md).[approve](chainify_evm.EvmNftProvider.md#approve)

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

#### Inherited from

[EvmNftProvider](chainify_evm.EvmNftProvider.md).[approveAll](chainify_evm.EvmNftProvider.md#approveall)

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

#### Inherited from

[EvmNftProvider](chainify_evm.EvmNftProvider.md).[balanceOf](chainify_evm.EvmNftProvider.md#balanceof)

#### Defined in

[evm/lib/nft/EvmNftProvider.ts:73](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/nft/EvmNftProvider.ts#L73)

___

### fetch

▸ **fetch**(): `Promise`<`NFTAsset`[]\>

#### Returns

`Promise`<`NFTAsset`[]\>

#### Overrides

[EvmNftProvider](chainify_evm.EvmNftProvider.md).[fetch](chainify_evm.EvmNftProvider.md#fetch)

#### Defined in

[evm/lib/nft/CovalentNftProvider.ts:22](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/nft/CovalentNftProvider.ts#L22)

___

### getWallet

▸ **getWallet**(): `default`<`BaseProvider`, `Signer`\>

#### Returns

`default`<`BaseProvider`, `Signer`\>

#### Inherited from

[EvmNftProvider](chainify_evm.EvmNftProvider.md).[getWallet](chainify_evm.EvmNftProvider.md#getwallet)

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

#### Inherited from

[EvmNftProvider](chainify_evm.EvmNftProvider.md).[isApprovedForAll](chainify_evm.EvmNftProvider.md#isapprovedforall)

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

[EvmNftProvider](chainify_evm.EvmNftProvider.md).[setWallet](chainify_evm.EvmNftProvider.md#setwallet)

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

#### Inherited from

[EvmNftProvider](chainify_evm.EvmNftProvider.md).[transfer](chainify_evm.EvmNftProvider.md#transfer)

#### Defined in

[evm/lib/nft/EvmNftProvider.ts:31](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/nft/EvmNftProvider.ts#L31)
