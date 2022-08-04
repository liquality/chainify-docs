---
id: "chainify_bitcoin.BitcoinSwapBaseProvider"
title: "Class: BitcoinSwapBaseProvider"
sidebar_label: "BitcoinSwapBaseProvider"
custom_edit_url: null
---

[@chainify/bitcoin](../modules/chainify_bitcoin.md).BitcoinSwapBaseProvider

## Hierarchy

- `default`<[`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md), ``null``, `IBitcoinWallet`<[`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md)\>\>

  ↳ **`BitcoinSwapBaseProvider`**

  ↳↳ [`BitcoinSwapEsploraProvider`](chainify_bitcoin.BitcoinSwapEsploraProvider.md)

  ↳↳ [`BitcoinSwapRpcProvider`](chainify_bitcoin.BitcoinSwapRpcProvider.md)

## Constructors

### constructor

• **new BitcoinSwapBaseProvider**(`options`, `walletProvider?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`BitcoinSwapProviderOptions`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinSwapProviderOptions.md) |
| `walletProvider?` | `IBitcoinWallet`<[`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md), `any`\> |

#### Overrides

Swap&lt;BitcoinBaseChainProvider, null, IBitcoinWallet&lt;BitcoinBaseChainProvider\&gt;\&gt;.constructor

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:22](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L22)

## Properties

### \_mode

• `Protected` **\_mode**: [`SwapMode`](../enums/chainify_bitcoin.BitcoinTypes.SwapMode.md)

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:20](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L20)

___

### \_network

• `Protected` **\_network**: [`BitcoinNetwork`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinNetwork.md)

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:19](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L19)

___

### walletProvider

• `Protected` **walletProvider**: `IBitcoinWallet`<[`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md), `any`\>

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

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:359](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L359)

___

### claimSwap

▸ **claimSwap**(`swapParams`, `initiationTxHash`, `secret`, `feePerByte`): `Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initiationTxHash` | `string` |
| `secret` | `string` |
| `feePerByte` | `number` |

#### Returns

`Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Overrides

Swap.claimSwap

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:53](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L53)

___

### doesTransactionMatchInitiation

▸ `Protected` **doesTransactionMatchInitiation**(`swapParams`, `transaction`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `transaction` | `Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\> |

#### Returns

`boolean`

#### Overrides

Swap.doesTransactionMatchInitiation

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:414](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L414)

___

### doesTransactionMatchRedeem

▸ `Protected` **doesTransactionMatchRedeem**(`initiationTxHash`, `tx`, `isRefund`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `initiationTxHash` | `string` |
| `tx` | `Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\> |
| `isRefund` | `boolean` |

#### Returns

`boolean`

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:401](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L401)

___

### extractSwapParams

▸ `Protected` **extractSwapParams**(`outputScript`): `Object`

#### Parameters

| Name | Type |
| :------ | :------ |
| `outputScript` | `string` |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `expiration` | `number` |
| `recipientPublicKey` | `string` |
| `refundPublicKey` | `string` |
| `secretHash` | `string` |

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:329](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L329)

___

### findClaimSwapTransaction

▸ **findClaimSwapTransaction**(`swapParams`, `initTxHash`, `blockNumber?`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTxHash` | `string` |
| `blockNumber?` | `number` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Overrides

Swap.findClaimSwapTransaction

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:90](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L90)

___

### findInitiateSwapTransaction

▸ **findInitiateSwapTransaction**(`swapParams`, `blockNumber?`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `blockNumber?` | `number` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Overrides

Swap.findInitiateSwapTransaction

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:67](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L67)

___

### findRefundSwapTransaction

▸ **findRefundSwapTransaction**(`swapParams`, `initiationTxHash`, `blockNumber?`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initiationTxHash` | `string` |
| `blockNumber?` | `number` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Overrides

Swap.findRefundSwapTransaction

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:111](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L111)

___

### findSwapTransaction

▸ `Protected` `Abstract` **findSwapTransaction**(`swapParams`, `blockNumber`, `predicate`): `Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `blockNumber` | `number` |
| `predicate` | [`TransactionMatchesFunction`](../namespaces/chainify_bitcoin.BitcoinTypes.md#transactionmatchesfunction) |

#### Returns

`Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:427](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L427)

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

### getInputScript

▸ `Protected` **getInputScript**(`vin`): `string`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `vin` | [`Input`](../interfaces/chainify_bitcoin.BitcoinTypes.Input.md) |

#### Returns

`string`[]

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:394](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L394)

___

### getSwapOutput

▸ `Protected` **getSwapOutput**(`swapParams`): `Buffer`

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |

#### Returns

`Buffer`

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:128](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L128)

___

### getSwapPaymentVariants

▸ `Protected` **getSwapPaymentVariants**(`swapOutput`): `Object`

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapOutput` | `Buffer` |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `p2sh` | `Payment` |
| `p2shSegwit` | `Payment` |
| `p2wsh` | `Payment` |

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:173](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L173)

___

### getSwapSecret

▸ **getSwapSecret**(`claimTxHash`, `initTxHash`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `claimTxHash` | `string` |
| `initTxHash` | `string` |

#### Returns

`Promise`<`string`\>

#### Overrides

Swap.getSwapSecret

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:74](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L74)

___

### getWallet

▸ **getWallet**(): `IBitcoinWallet`<[`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md), `any`\>

#### Returns

`IBitcoinWallet`<[`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md), `any`\>

#### Inherited from

Swap.getWallet

#### Defined in

client/dist/lib/Swap.d.ts:7

___

### initiateSwap

▸ **initiateSwap**(`swapParams`, `feePerByte`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `feePerByte` | `number` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Overrides

Swap.initiateSwap

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:41](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L41)

___

### onWalletProviderUpdate

▸ `Protected` **onWalletProviderUpdate**(`_wallet`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `_wallet` | `IBitcoinWallet`<[`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md), `any`\> |

#### Returns

`void`

#### Overrides

Swap.onWalletProviderUpdate

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:124](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L124)

___

### refundSwap

▸ **refundSwap**(`swapParams`, `initiationTxHash`, `feePerByte`): `Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initiationTxHash` | `string` |
| `feePerByte` | `number` |

#### Returns

`Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Overrides

Swap.refundSwap

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:61](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L61)

___

### setWallet

▸ **setWallet**(`wallet`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `wallet` | `IBitcoinWallet`<[`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md), `any`\> |

#### Returns

`void`

#### Inherited from

Swap.setWallet

#### Defined in

client/dist/lib/Swap.d.ts:6

___

### updateTransactionFee

▸ **updateTransactionFee**(`tx`, `newFeePerByte`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `tx` | `string` \| `Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\> |
| `newFeePerByte` | `number` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Overrides

Swap.updateTransactionFee

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:363](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L363)

___

### validateSwapParams

▸ **validateSwapParams**(`swapParams`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |

#### Returns

`void`

#### Overrides

Swap.validateSwapParams

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:33](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L33)

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
