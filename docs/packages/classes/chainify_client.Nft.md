---
id: "chainify_client.Nft"
title: "Class: Nft<T, S>"
sidebar_label: "Nft"
custom_edit_url: null
---

[@chainify/client](../modules/chainify_client.md).Nft

## Type parameters

| Name |
| :------ |
| `T` |
| `S` |

## Constructors

### constructor

• **new Nft**<`T`, `S`\>(`walletProvider?`)

#### Type parameters

| Name |
| :------ |
| `T` |
| `S` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `walletProvider?` | [`Wallet`](chainify_client.Wallet.md)<`T`, `S`\> |

#### Defined in

[client/lib/Nft.ts:7](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Nft.ts#L7)

## Properties

### walletProvider

• `Protected` **walletProvider**: [`Wallet`](chainify_client.Wallet.md)<`T`, `S`\>

#### Defined in

[client/lib/Nft.ts:5](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Nft.ts#L5)

## Methods

### approve

▸ `Abstract` **approve**(`contract`, `operator`, `tokenID`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `contract` | `AddressType` |
| `operator` | `AddressType` |
| `tokenID` | `number` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Defined in

[client/lib/Nft.ts:30](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Nft.ts#L30)

___

### approveAll

▸ `Abstract` **approveAll**(`contract`, `operator`, `state`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `contract` | `AddressType` |
| `operator` | `AddressType` |
| `state` | `boolean` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Defined in

[client/lib/Nft.ts:32](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Nft.ts#L32)

___

### balanceOf

▸ `Abstract` **balanceOf**(`contractAddress`, `owners`, `tokenIDs`): `Promise`<`BigNumber` \| `BigNumber`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `contractAddress` | `AddressType` |
| `owners` | `AddressType`[] |
| `tokenIDs` | `number`[] |

#### Returns

`Promise`<`BigNumber` \| `BigNumber`[]\>

#### Defined in

[client/lib/Nft.ts:28](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Nft.ts#L28)

___

### fetch

▸ `Abstract` **fetch**(): `Promise`<`NFTAsset`[]\>

#### Returns

`Promise`<`NFTAsset`[]\>

#### Defined in

[client/lib/Nft.ts:36](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Nft.ts#L36)

___

### getWallet

▸ **getWallet**(): [`Wallet`](chainify_client.Wallet.md)<`T`, `S`\>

#### Returns

[`Wallet`](chainify_client.Wallet.md)<`T`, `S`\>

#### Defined in

[client/lib/Nft.ts:15](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Nft.ts#L15)

___

### isApprovedForAll

▸ `Abstract` **isApprovedForAll**(`contract`, `operator`): `Promise`<`boolean`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `contract` | `AddressType` |
| `operator` | `AddressType` |

#### Returns

`Promise`<`boolean`\>

#### Defined in

[client/lib/Nft.ts:34](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Nft.ts#L34)

___

### setWallet

▸ **setWallet**(`wallet`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `wallet` | [`Wallet`](chainify_client.Wallet.md)<`T`, `S`\> |

#### Returns

`void`

#### Defined in

[client/lib/Nft.ts:11](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Nft.ts#L11)

___

### transfer

▸ `Abstract` **transfer**(`contract`, `receiver`, `tokenIDs`, `values?`, `data?`, `fee?`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `contract` | `AddressType` |
| `receiver` | `AddressType` |
| `tokenIDs` | `string`[] |
| `values?` | `number`[] |
| `data?` | `string` |
| `fee?` | `FeeType` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Defined in

[client/lib/Nft.ts:19](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Nft.ts#L19)
