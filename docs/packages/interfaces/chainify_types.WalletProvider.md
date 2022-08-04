---
id: "chainify_types.WalletProvider"
title: "Interface: WalletProvider"
sidebar_label: "WalletProvider"
custom_edit_url: null
---

[@chainify/types](../modules/chainify_types.md).WalletProvider

## Properties

### canUpdateFee

• `Optional` **canUpdateFee**: `boolean` \| () => `boolean`

#### Defined in

[types/lib/Wallet.ts:32](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Wallet.ts#L32)

## Methods

### exportPrivateKey

▸ `Optional` **exportPrivateKey**(): `Promise`<`string`\>

#### Returns

`Promise`<`string`\>

#### Defined in

[types/lib/Wallet.ts:34](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Wallet.ts#L34)

___

### getAddresses

▸ **getAddresses**(`startingIndex?`, `numAddresses?`, `change?`): `Promise`<[`Address`](../classes/chainify_types.Address.md)[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `startingIndex?` | `number` |
| `numAddresses?` | `number` |
| `change?` | `boolean` |

#### Returns

`Promise`<[`Address`](../classes/chainify_types.Address.md)[]\>

#### Defined in

[types/lib/Wallet.ts:12](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Wallet.ts#L12)

___

### getConnectedNetwork

▸ **getConnectedNetwork**(): `Promise`<`any`\>

#### Returns

`Promise`<`any`\>

#### Defined in

[types/lib/Wallet.ts:28](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Wallet.ts#L28)

___

### getUnusedAddress

▸ **getUnusedAddress**(`change?`, `numAddressPerCall?`): `Promise`<[`Address`](../classes/chainify_types.Address.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `change?` | `boolean` |
| `numAddressPerCall?` | `number` |

#### Returns

`Promise`<[`Address`](../classes/chainify_types.Address.md)\>

#### Defined in

[types/lib/Wallet.ts:24](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Wallet.ts#L24)

___

### getUsedAddresses

▸ **getUsedAddresses**(`numAddressPerCall?`): `Promise`<[`Address`](../classes/chainify_types.Address.md)[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `numAddressPerCall?` | `number` |

#### Returns

`Promise`<[`Address`](../classes/chainify_types.Address.md)[]\>

#### Defined in

[types/lib/Wallet.ts:14](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Wallet.ts#L14)

___

### isWalletAvailable

▸ **isWalletAvailable**(): `Promise`<`boolean`\>

#### Returns

`Promise`<`boolean`\>

#### Defined in

[types/lib/Wallet.ts:30](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Wallet.ts#L30)

___

### sendBatchTransaction

▸ **sendBatchTransaction**(`transactions`): `Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `transactions` | [`TransactionRequest`](../modules/chainify_types.md#transactionrequest)[] |

#### Returns

`Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>[]\>

#### Defined in

[types/lib/Wallet.ts:22](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Wallet.ts#L22)

___

### sendSweepTransaction

▸ **sendSweepTransaction**(`address`, `asset`, `fee?`): `Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | [`AddressType`](../modules/chainify_types.md#addresstype) |
| `asset` | [`Asset`](chainify_types.Asset.md) |
| `fee?` | [`FeeType`](../modules/chainify_types.md#feetype) |

#### Returns

`Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Defined in

[types/lib/Wallet.ts:18](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Wallet.ts#L18)

___

### sendTransaction

▸ **sendTransaction**(`options`): `Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`TransactionRequest`](../modules/chainify_types.md#transactionrequest) |

#### Returns

`Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Defined in

[types/lib/Wallet.ts:16](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Wallet.ts#L16)

___

### signMessage

▸ **signMessage**(`message`, `from`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `from` | `string` |

#### Returns

`Promise`<`string`\>

#### Defined in

[types/lib/Wallet.ts:26](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Wallet.ts#L26)

___

### updateTransactionFee

▸ **updateTransactionFee**(`tx`, `newFee`): `Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `tx` | `string` \| [`Transaction`](chainify_types.Transaction.md)<`any`\> |
| `newFee` | [`FeeType`](../modules/chainify_types.md#feetype) |

#### Returns

`Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Defined in

[types/lib/Wallet.ts:20](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Wallet.ts#L20)
