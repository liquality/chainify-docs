---
id: "chainify_near.NearUtils"
title: "Namespace: NearUtils"
sidebar_label: "NearUtils"
custom_edit_url: null
---

[@chainify/near](../modules/chainify_near.md).NearUtils

## Functions

### getClaimActions

▸ **getClaimActions**(`secret`): `Action`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `secret` | `string` |

#### Returns

`Action`[]

#### Defined in

[near/lib/utils.ts:75](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/utils.ts#L75)

___

### getHtlcActions

▸ **getHtlcActions**(`swapParams`): `Action`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |

#### Returns

`Action`[]

#### Defined in

[near/lib/utils.ts:66](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/utils.ts#L66)

___

### getRefundActions

▸ **getRefundActions**(): `Action`[]

#### Returns

`Action`[]

#### Defined in

[near/lib/utils.ts:80](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/utils.ts#L80)

___

### parseBlockResponse

▸ **parseBlockResponse**(`block`, `transactions?`): `Block`<`BlockResult`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `block` | `BlockResult` |
| `transactions?` | `Transaction`<`any`\>[] |

#### Returns

`Block`<`BlockResult`\>

#### Defined in

[near/lib/utils.ts:7](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/utils.ts#L7)

___

### parseNearBlockTx

▸ **parseNearBlockTx**(`tx`, `currentBlock`, `txBlock`): `Transaction`<[`NearTransaction`](../interfaces/chainify_near.NearTypes.NearTransaction.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `tx` | [`NearTransaction`](../interfaces/chainify_near.NearTypes.NearTransaction.md) |
| `currentBlock` | `number` |
| `txBlock` | `number` |

#### Returns

`Transaction`<[`NearTransaction`](../interfaces/chainify_near.NearTypes.NearTransaction.md)\>

#### Defined in

[near/lib/utils.ts:19](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/utils.ts#L19)

___

### parseScraperTransaction

▸ **parseScraperTransaction**(`tx`): [`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `tx` | [`NearScraperData`](../interfaces/chainify_near.NearTypes.NearScraperData.md) |

#### Returns

[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)

#### Defined in

[near/lib/utils.ts:85](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/utils.ts#L85)

___

### parseTxResponse

▸ **parseTxResponse**(`response`, `blockNumber?`, `latestBlock?`): `Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `response` | [`NearTxResponse`](../interfaces/chainify_near.NearTypes.NearTxResponse.md) |
| `blockNumber?` | `number` |
| `latestBlock?` | `number` |

#### Returns

`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>

#### Defined in

[near/lib/utils.ts:29](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/utils.ts#L29)
