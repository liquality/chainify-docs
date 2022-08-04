---
id: "chainify_types.SwapProvider"
title: "Interface: SwapProvider"
sidebar_label: "SwapProvider"
custom_edit_url: null
---

[@chainify/types](../modules/chainify_types.md).SwapProvider

## Methods

### claimSwap

▸ **claimSwap**(`swapParams`, `initiationTxHash`, `secret`, `fee`): `Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | [`SwapParams`](chainify_types.SwapParams.md) |
| `initiationTxHash` | `string` |
| `secret` | `string` |
| `fee` | [`FeeType`](../modules/chainify_types.md#feetype) |

#### Returns

`Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Defined in

[types/lib/Swap.ts:44](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Swap.ts#L44)

___

### findClaimSwapTransaction

▸ **findClaimSwapTransaction**(`swapParams`, `initiationTxHash`, `blockNumber?`): `Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | [`SwapParams`](chainify_types.SwapParams.md) |
| `initiationTxHash` | `string` |
| `blockNumber?` | `number` |

#### Returns

`Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Defined in

[types/lib/Swap.ts:32](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Swap.ts#L32)

___

### findInitiateSwapTransaction

▸ **findInitiateSwapTransaction**(`swapParams`, `blockNumber?`): `Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | [`SwapParams`](chainify_types.SwapParams.md) |
| `blockNumber?` | `number` |

#### Returns

`Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Defined in

[types/lib/Swap.ts:30](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Swap.ts#L30)

___

### findRefundSwapTransaction

▸ **findRefundSwapTransaction**(`swapParams`, `initiationTxHash`, `blockNumber?`): `Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | [`SwapParams`](chainify_types.SwapParams.md) |
| `initiationTxHash` | `string` |
| `blockNumber?` | `number` |

#### Returns

`Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Defined in

[types/lib/Swap.ts:34](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Swap.ts#L34)

___

### generateSecret

▸ **generateSecret**(`message`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |

#### Returns

`Promise`<`string`\>

#### Defined in

[types/lib/Swap.ts:36](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Swap.ts#L36)

___

### getSwapSecret

▸ **getSwapSecret**(`claimTxHash`, `initTxHash?`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `claimTxHash` | `string` |
| `initTxHash?` | `string` |

#### Returns

`Promise`<`string`\>

#### Defined in

[types/lib/Swap.ts:38](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Swap.ts#L38)

___

### initiateSwap

▸ **initiateSwap**(`swapParams`, `fee`): `Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | [`SwapParams`](chainify_types.SwapParams.md) |
| `fee` | [`FeeType`](../modules/chainify_types.md#feetype) |

#### Returns

`Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Defined in

[types/lib/Swap.ts:40](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Swap.ts#L40)

___

### refundSwap

▸ **refundSwap**(`swapParams`, `initiationTxHash`, `fee`): `Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | [`SwapParams`](chainify_types.SwapParams.md) |
| `initiationTxHash` | `string` |
| `fee` | [`FeeType`](../modules/chainify_types.md#feetype) |

#### Returns

`Promise`<[`Transaction`](chainify_types.Transaction.md)<`any`\>\>

#### Defined in

[types/lib/Swap.ts:46](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Swap.ts#L46)

___

### verifyInitiateSwapTransaction

▸ **verifyInitiateSwapTransaction**(`swapParams`, `initiationTxHash`): `Promise`<`boolean`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | [`SwapParams`](chainify_types.SwapParams.md) |
| `initiationTxHash` | `string` \| [`Transaction`](chainify_types.Transaction.md)<`any`\> |

#### Returns

`Promise`<`boolean`\>

#### Defined in

[types/lib/Swap.ts:42](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Swap.ts#L42)
