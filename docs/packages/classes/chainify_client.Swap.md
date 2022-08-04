---
id: "chainify_client.Swap"
title: "Class: Swap<T, S, WalletProvider>"
sidebar_label: "Swap"
custom_edit_url: null
---

[@chainify/client](../modules/chainify_client.md).Swap

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `T` |
| `S` | `S` |
| `WalletProvider` | extends [`Wallet`](chainify_client.Wallet.md)<`T`, `S`\> = [`Wallet`](chainify_client.Wallet.md)<`T`, `S`\> |

## Implements

- `SwapProvider`

## Constructors

### constructor

• **new Swap**<`T`, `S`, `WalletProvider`\>(`walletProvider?`)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `T` |
| `S` | `S` |
| `WalletProvider` | extends [`Wallet`](chainify_client.Wallet.md)<`T`, `S`, `WalletProvider`\> = [`Wallet`](chainify_client.Wallet.md)<`T`, `S`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `walletProvider?` | `WalletProvider` |

#### Defined in

[client/lib/Swap.ts:9](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L9)

## Properties

### walletProvider

• `Protected` **walletProvider**: `WalletProvider`

#### Defined in

[client/lib/Swap.ts:7](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L7)

## Methods

### canUpdateFee

▸ `Abstract` **canUpdateFee**(): `boolean`

#### Returns

`boolean`

#### Defined in

[client/lib/Swap.ts:71](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L71)

___

### claimSwap

▸ `Abstract` **claimSwap**(`swapParams`, `initTx`, `secret`, `fee?`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTx` | `string` |
| `secret` | `string` |
| `fee?` | `FeeType` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Implementation of

SwapProvider.claimSwap

#### Defined in

[client/lib/Swap.ts:63](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L63)

___

### doesTransactionMatchInitiation

▸ `Protected` `Abstract` **doesTransactionMatchInitiation**(`swapParams`, `transaction`): `boolean` \| `Promise`<`boolean`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `transaction` | `Transaction`<`any`\> |

#### Returns

`boolean` \| `Promise`<`boolean`\>

#### Defined in

[client/lib/Swap.ts:74](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L74)

___

### findClaimSwapTransaction

▸ `Abstract` **findClaimSwapTransaction**(`swapParams`, `initTxHash`, `blockNumber?`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTxHash` | `string` |
| `blockNumber?` | `number` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Implementation of

SwapProvider.findClaimSwapTransaction

#### Defined in

[client/lib/Swap.ts:64](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L64)

___

### findInitiateSwapTransaction

▸ `Abstract` **findInitiateSwapTransaction**(`swapParams`, `_blockNumber?`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `_blockNumber?` | `number` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Implementation of

SwapProvider.findInitiateSwapTransaction

#### Defined in

[client/lib/Swap.ts:61](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L61)

___

### findRefundSwapTransaction

▸ `Abstract` **findRefundSwapTransaction**(`swapParams`, `initiationTxHash`, `blockNumber?`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initiationTxHash` | `string` |
| `blockNumber?` | `number` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Implementation of

SwapProvider.findRefundSwapTransaction

#### Defined in

[client/lib/Swap.ts:67](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L67)

___

### generateSecret

▸ **generateSecret**(`message`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |

#### Returns

`Promise`<`string`\>

#### Implementation of

SwapProvider.generateSecret

#### Defined in

[client/lib/Swap.ts:53](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L53)

___

### getSwapSecret

▸ `Abstract` **getSwapSecret**(`claimTxHash`, `initTxHash?`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `claimTxHash` | `string` |
| `initTxHash?` | `string` |

#### Returns

`Promise`<`string`\>

#### Implementation of

SwapProvider.getSwapSecret

#### Defined in

[client/lib/Swap.ts:69](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L69)

___

### getWallet

▸ **getWallet**(): `WalletProvider`

#### Returns

`WalletProvider`

#### Defined in

[client/lib/Swap.ts:18](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L18)

___

### initiateSwap

▸ `Abstract` **initiateSwap**(`swapParams`, `fee?`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `fee?` | `FeeType` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Implementation of

SwapProvider.initiateSwap

#### Defined in

[client/lib/Swap.ts:60](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L60)

___

### onWalletProviderUpdate

▸ `Protected` `Abstract` **onWalletProviderUpdate**(`wallet`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `wallet` | `WalletProvider` |

#### Returns

`void`

#### Defined in

[client/lib/Swap.ts:76](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L76)

___

### refundSwap

▸ `Abstract` **refundSwap**(`swapParams`, `initTx`, `fee?`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTx` | `string` |
| `fee?` | `FeeType` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Implementation of

SwapProvider.refundSwap

#### Defined in

[client/lib/Swap.ts:66](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L66)

___

### setWallet

▸ **setWallet**(`wallet`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `wallet` | `WalletProvider` |

#### Returns

`void`

#### Defined in

[client/lib/Swap.ts:13](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L13)

___

### updateTransactionFee

▸ `Abstract` **updateTransactionFee**(`tx`, `newFee`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `tx` | `string` \| `Transaction`<`any`\> |
| `newFee` | `FeeType` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Defined in

[client/lib/Swap.ts:72](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L72)

___

### validateSwapParams

▸ **validateSwapParams**(`swapParams`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |

#### Returns

`void`

#### Defined in

[client/lib/Swap.ts:47](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L47)

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

#### Implementation of

SwapProvider.verifyInitiateSwapTransaction

#### Defined in

[client/lib/Swap.ts:22](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Swap.ts#L22)
