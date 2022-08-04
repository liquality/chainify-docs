---
id: "chainify_near.NearSwapProvider"
title: "Class: NearSwapProvider"
sidebar_label: "NearSwapProvider"
custom_edit_url: null
---

[@chainify/near](../modules/chainify_near.md).NearSwapProvider

## Hierarchy

- `default`<`providers.JsonRpcProvider`, `InMemorySigner`\>

  ↳ **`NearSwapProvider`**

## Constructors

### constructor

• **new NearSwapProvider**(`helperUrl`, `walletProvider?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `helperUrl` | `string` |
| `walletProvider?` | `default`<`JsonRpcProvider`, `InMemorySigner`\> |

#### Overrides

Swap&lt;providers.JsonRpcProvider, InMemorySigner\&gt;.constructor

#### Defined in

[near/lib/swap/NearSwapProvider.ts:14](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/swap/NearSwapProvider.ts#L14)

## Properties

### walletProvider

• `Protected` **walletProvider**: `default`<`JsonRpcProvider`, `InMemorySigner`\>

#### Inherited from

Swap.walletProvider

#### Defined in

client/dist/lib/Swap.d.ts:4

## Methods

### canUpdateFee

▸ **canUpdateFee**(): `boolean`

#### Returns

`boolean`

#### Overrides

Swap.canUpdateFee

#### Defined in

[near/lib/swap/NearSwapProvider.ts:151](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/swap/NearSwapProvider.ts#L151)

___

### claimSwap

▸ **claimSwap**(`swapParams`, `initTxHash`, `secret`): `Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTxHash` | `string` |
| `secret` | `string` |

#### Returns

`Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Overrides

Swap.claimSwap

#### Defined in

[near/lib/swap/NearSwapProvider.ts:34](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/swap/NearSwapProvider.ts#L34)

___

### doesTransactionMatchInitiation

▸ `Protected` **doesTransactionMatchInitiation**(`swapParams`, `transaction`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `transaction` | `Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\> |

#### Returns

`boolean`

#### Overrides

Swap.doesTransactionMatchInitiation

#### Defined in

[near/lib/swap/NearSwapProvider.ts:98](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/swap/NearSwapProvider.ts#L98)

___

### findClaimSwapTransaction

▸ **findClaimSwapTransaction**(`swapParams`, `initTxHash`): `Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTxHash` | `string` |

#### Returns

`Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Overrides

Swap.findClaimSwapTransaction

#### Defined in

[near/lib/swap/NearSwapProvider.ts:48](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/swap/NearSwapProvider.ts#L48)

___

### findInitiateSwapTransaction

▸ **findInitiateSwapTransaction**(`swapParams`, `_blockNumber?`): `Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `_blockNumber?` | `number` |

#### Returns

`Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Overrides

Swap.findInitiateSwapTransaction

#### Defined in

[near/lib/swap/NearSwapProvider.ts:28](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/swap/NearSwapProvider.ts#L28)

___

### findRefundSwapTransaction

▸ **findRefundSwapTransaction**(`swapParams`, `initTxHash`): `Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTxHash` | `string` |

#### Returns

`Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Overrides

Swap.findRefundSwapTransaction

#### Defined in

[near/lib/swap/NearSwapProvider.ts:76](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/swap/NearSwapProvider.ts#L76)

___

### generateSecret

▸ **generateSecret**(`message`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |

#### Returns

`Promise`<`string`\>

#### Inherited from

Swap.generateSecret

#### Defined in

client/dist/lib/Swap.d.ts:10

___

### getSwapSecret

▸ **getSwapSecret**(`claimTxHash`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `claimTxHash` | `string` |

#### Returns

`Promise`<`string`\>

#### Overrides

Swap.getSwapSecret

#### Defined in

[near/lib/swap/NearSwapProvider.ts:86](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/swap/NearSwapProvider.ts#L86)

___

### getWallet

▸ **getWallet**(): `default`<`JsonRpcProvider`, `InMemorySigner`\>

#### Returns

`default`<`JsonRpcProvider`, `InMemorySigner`\>

#### Inherited from

Swap.getWallet

#### Defined in

client/dist/lib/Swap.d.ts:7

___

### initiateSwap

▸ **initiateSwap**(`swapParams`): `Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |

#### Returns

`Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Overrides

Swap.initiateSwap

#### Defined in

[near/lib/swap/NearSwapProvider.ts:19](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/swap/NearSwapProvider.ts#L19)

___

### onWalletProviderUpdate

▸ `Protected` **onWalletProviderUpdate**(`_wallet`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `_wallet` | `default`<`JsonRpcProvider`, `InMemorySigner`\> |

#### Returns

`void`

#### Overrides

Swap.onWalletProviderUpdate

#### Defined in

[near/lib/swap/NearSwapProvider.ts:94](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/swap/NearSwapProvider.ts#L94)

___

### refundSwap

▸ **refundSwap**(`swapParams`, `initTxHash`): `Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTxHash` | `string` |

#### Returns

`Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Overrides

Swap.refundSwap

#### Defined in

[near/lib/swap/NearSwapProvider.ts:65](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/swap/NearSwapProvider.ts#L65)

___

### setWallet

▸ **setWallet**(`wallet`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `wallet` | `default`<`JsonRpcProvider`, `InMemorySigner`\> |

#### Returns

`void`

#### Inherited from

Swap.setWallet

#### Defined in

client/dist/lib/Swap.d.ts:6

___

### updateTransactionFee

▸ **updateTransactionFee**(`_tx`, `_newFee`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_tx` | `string` \| `Transaction`<`any`\> |
| `_newFee` | `FeeType` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Overrides

Swap.updateTransactionFee

#### Defined in

[near/lib/swap/NearSwapProvider.ts:155](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/swap/NearSwapProvider.ts#L155)

___

### validateSwapParams

▸ **validateSwapParams**(`swapParams`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |

#### Returns

`void`

#### Inherited from

Swap.validateSwapParams

#### Defined in

client/dist/lib/Swap.d.ts:9

___

### verifyInitiateSwapTransaction

▸ **verifyInitiateSwapTransaction**(`swapParams`, `initTx`): `Promise`<`boolean`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTx` | `string` \| `Transaction`<`any`\> |

#### Returns

`Promise`<`boolean`\>

#### Inherited from

Swap.verifyInitiateSwapTransaction

#### Defined in

client/dist/lib/Swap.d.ts:8
