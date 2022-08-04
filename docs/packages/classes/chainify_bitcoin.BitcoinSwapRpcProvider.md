---
id: "chainify_bitcoin.BitcoinSwapRpcProvider"
title: "Class: BitcoinSwapRpcProvider"
sidebar_label: "BitcoinSwapRpcProvider"
custom_edit_url: null
---

[@chainify/bitcoin](../modules/chainify_bitcoin.md).BitcoinSwapRpcProvider

## Hierarchy

- [`BitcoinSwapBaseProvider`](chainify_bitcoin.BitcoinSwapBaseProvider.md)

  ↳ **`BitcoinSwapRpcProvider`**

## Constructors

### constructor

• **new BitcoinSwapRpcProvider**(`options`, `walletProvider?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`BitcoinSwapProviderOptions`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinSwapProviderOptions.md) |
| `walletProvider?` | `IBitcoinWallet`<[`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md), `any`\> |

#### Overrides

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[constructor](chainify_bitcoin.BitcoinSwapBaseProvider.md#constructor)

#### Defined in

[bitcoin/lib/swap/BitcoinSwapRpcProvider.ts:9](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapRpcProvider.ts#L9)

## Properties

### \_mode

• `Protected` **\_mode**: [`SwapMode`](../enums/chainify_bitcoin.BitcoinTypes.SwapMode.md)

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[_mode](chainify_bitcoin.BitcoinSwapBaseProvider.md#_mode)

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:20](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L20)

___

### \_network

• `Protected` **\_network**: [`BitcoinNetwork`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinNetwork.md)

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[_network](chainify_bitcoin.BitcoinSwapBaseProvider.md#_network)

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:19](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L19)

___

### walletProvider

• `Protected` **walletProvider**: `IBitcoinWallet`<[`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md), `any`\>

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[walletProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md#walletprovider)

#### Defined in

client/dist/lib/Swap.d.ts:4

## Methods

### canUpdateFee

▸ **canUpdateFee**(): `boolean`

#### Returns

`boolean`

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[canUpdateFee](chainify_bitcoin.BitcoinSwapBaseProvider.md#canupdatefee)

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

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[claimSwap](chainify_bitcoin.BitcoinSwapBaseProvider.md#claimswap)

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

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[doesTransactionMatchInitiation](chainify_bitcoin.BitcoinSwapBaseProvider.md#doestransactionmatchinitiation)

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

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[doesTransactionMatchRedeem](chainify_bitcoin.BitcoinSwapBaseProvider.md#doestransactionmatchredeem)

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

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[extractSwapParams](chainify_bitcoin.BitcoinSwapBaseProvider.md#extractswapparams)

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

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[findClaimSwapTransaction](chainify_bitcoin.BitcoinSwapBaseProvider.md#findclaimswaptransaction)

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

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[findInitiateSwapTransaction](chainify_bitcoin.BitcoinSwapBaseProvider.md#findinitiateswaptransaction)

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

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[findRefundSwapTransaction](chainify_bitcoin.BitcoinSwapBaseProvider.md#findrefundswaptransaction)

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:111](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L111)

___

### findSwapTransaction

▸ **findSwapTransaction**(`_swapParams`, `blockNumber`, `predicate`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_swapParams` | `SwapParams` |
| `blockNumber` | `number` |
| `predicate` | (`tx`: `Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>) => `boolean` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Overrides

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[findSwapTransaction](chainify_bitcoin.BitcoinSwapBaseProvider.md#findswaptransaction)

#### Defined in

[bitcoin/lib/swap/BitcoinSwapRpcProvider.ts:13](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapRpcProvider.ts#L13)

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

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[generateSecret](chainify_bitcoin.BitcoinSwapBaseProvider.md#generatesecret)

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

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[getInputScript](chainify_bitcoin.BitcoinSwapBaseProvider.md#getinputscript)

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

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[getSwapOutput](chainify_bitcoin.BitcoinSwapBaseProvider.md#getswapoutput)

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

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[getSwapPaymentVariants](chainify_bitcoin.BitcoinSwapBaseProvider.md#getswappaymentvariants)

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

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[getSwapSecret](chainify_bitcoin.BitcoinSwapBaseProvider.md#getswapsecret)

#### Defined in

[bitcoin/lib/swap/BitcoinSwapBaseProvider.ts:74](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/BitcoinSwapBaseProvider.ts#L74)

___

### getWallet

▸ **getWallet**(): `IBitcoinWallet`<[`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md), `any`\>

#### Returns

`IBitcoinWallet`<[`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md), `any`\>

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[getWallet](chainify_bitcoin.BitcoinSwapBaseProvider.md#getwallet)

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

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[initiateSwap](chainify_bitcoin.BitcoinSwapBaseProvider.md#initiateswap)

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

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[onWalletProviderUpdate](chainify_bitcoin.BitcoinSwapBaseProvider.md#onwalletproviderupdate)

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

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[refundSwap](chainify_bitcoin.BitcoinSwapBaseProvider.md#refundswap)

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

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[setWallet](chainify_bitcoin.BitcoinSwapBaseProvider.md#setwallet)

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

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[updateTransactionFee](chainify_bitcoin.BitcoinSwapBaseProvider.md#updatetransactionfee)

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

#### Inherited from

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[validateSwapParams](chainify_bitcoin.BitcoinSwapBaseProvider.md#validateswapparams)

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

[BitcoinSwapBaseProvider](chainify_bitcoin.BitcoinSwapBaseProvider.md).[verifyInitiateSwapTransaction](chainify_bitcoin.BitcoinSwapBaseProvider.md#verifyinitiateswaptransaction)

#### Defined in

client/dist/lib/Swap.d.ts:8
