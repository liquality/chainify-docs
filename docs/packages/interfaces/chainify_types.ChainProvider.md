---
id: "chainify_types.ChainProvider"
title: "Interface: ChainProvider"
sidebar_label: "ChainProvider"
custom_edit_url: null
---

[@chainify/types](../modules/chainify_types.md).ChainProvider

## Methods

### getBalance

▸ **getBalance**(`addresses`, `assets`): `Promise`<`BigNumber`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `addresses` | [`AddressType`](../modules/chainify_types.md#addresstype)[] |
| `assets` | [`Asset`](chainify_types.Asset.md)[] |

#### Returns

`Promise`<`BigNumber`[]\>

#### Defined in

[types/lib/Chain.ts:15](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Chain.ts#L15)

___

### getBlockByHash

▸ **getBlockByHash**(`blockHash`, `includeTx?`): `Promise`<[`Block`](chainify_types.Block.md)<`any`, `any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `blockHash` | `string` |
| `includeTx?` | `boolean` |

#### Returns

`Promise`<[`Block`](chainify_types.Block.md)<`any`, `any`\>\>

#### Defined in

[types/lib/Chain.ts:7](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Chain.ts#L7)

___

### getBlockByNumber

▸ **getBlockByNumber**(`blockNumber`, `includeTx?`): `Promise`<[`Block`](chainify_types.Block.md)<`any`, `any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `blockNumber` | `number` |
| `includeTx?` | `boolean` |

#### Returns

`Promise`<[`Block`](chainify_types.Block.md)<`any`, `any`\>\>

#### Defined in

[types/lib/Chain.ts:9](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Chain.ts#L9)

___

### getBlockHeight

▸ **getBlockHeight**(): `Promise`<`number`\>

#### Returns

`Promise`<`number`\>

#### Defined in

[types/lib/Chain.ts:11](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Chain.ts#L11)

___

### getTransactionByHash

▸ **getTransactionByHash**(`txHash`): `Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txHash` | `string` |

#### Returns

`Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Defined in

[types/lib/Chain.ts:13](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Chain.ts#L13)
