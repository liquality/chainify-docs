---
id: "chainify_evm.EvmSwapProvider"
title: "Class: EvmSwapProvider"
sidebar_label: "EvmSwapProvider"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).EvmSwapProvider

## Hierarchy

- [`EvmBaseSwapProvider`](chainify_evm.EvmBaseSwapProvider.md)

  ↳ **`EvmSwapProvider`**

## Constructors

### constructor

• **new EvmSwapProvider**(`swapOptions`, `walletProvider?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapOptions` | [`EvmSwapOptions`](../interfaces/chainify_evm.EvmTypes.EvmSwapOptions.md) |
| `walletProvider?` | [`EvmBaseWalletProvider`](chainify_evm.EvmBaseWalletProvider.md)<`BaseProvider`, `Signer`\> |

#### Overrides

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[constructor](chainify_evm.EvmBaseSwapProvider.md#constructor)

#### Defined in

[evm/lib/swap/EvmSwapProvider.ts:12](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmSwapProvider.ts#L12)

## Properties

### contract

• `Protected` **contract**: [`LiqualityHTLC`](../interfaces/chainify_evm.Typechain.LiqualityHTLC.md)

#### Inherited from

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[contract](chainify_evm.EvmBaseSwapProvider.md#contract)

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:16](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L16)

___

### swapOptions

• `Protected` **swapOptions**: [`EvmSwapOptions`](../interfaces/chainify_evm.EvmTypes.EvmSwapOptions.md)

#### Inherited from

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[swapOptions](chainify_evm.EvmBaseSwapProvider.md#swapoptions)

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:17](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L17)

___

### walletProvider

• `Protected` **walletProvider**: [`EvmBaseWalletProvider`](chainify_evm.EvmBaseWalletProvider.md)<`BaseProvider`, `Signer`\>

#### Overrides

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[walletProvider](chainify_evm.EvmBaseSwapProvider.md#walletprovider)

#### Defined in

[evm/lib/swap/EvmSwapProvider.ts:10](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmSwapProvider.ts#L10)

## Methods

### canUpdateFee

▸ **canUpdateFee**(): `boolean`

#### Returns

`boolean`

#### Inherited from

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[canUpdateFee](chainify_evm.EvmBaseSwapProvider.md#canupdatefee)

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:119](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L119)

___

### claimSwap

▸ **claimSwap**(`swapParams`, `initTxHash`, `secret`, `fee`): `Promise`<`Transaction`<`TransactionResponse`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTxHash` | `string` |
| `secret` | `string` |
| `fee` | `FeeType` |

#### Returns

`Promise`<`Transaction`<`TransactionResponse`\>\>

#### Inherited from

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[claimSwap](chainify_evm.EvmBaseSwapProvider.md#claimswap)

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:46](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L46)

___

### doesTransactionMatchInitiation

▸ `Protected` **doesTransactionMatchInitiation**(`swapParams`, `transaction`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `transaction` | `Transaction`<`InitiateEvent`\> |

#### Returns

`boolean`

#### Inherited from

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[doesTransactionMatchInitiation](chainify_evm.EvmBaseSwapProvider.md#doestransactionmatchinitiation)

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:131](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L131)

___

### findClaimSwapTransaction

▸ **findClaimSwapTransaction**(`swapParams`, `initTxHash`): `Promise`<`Transaction`<`ClaimEvent`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTxHash` | `string` |

#### Returns

`Promise`<`Transaction`<`ClaimEvent`\>\>

#### Overrides

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[findClaimSwapTransaction](chainify_evm.EvmBaseSwapProvider.md#findclaimswaptransaction)

#### Defined in

[evm/lib/swap/EvmSwapProvider.ts:36](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmSwapProvider.ts#L36)

___

### findInitiateSwapTransaction

▸ **findInitiateSwapTransaction**(`swapParams`): `Promise`<`Transaction`<`InitiateEvent`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |

#### Returns

`Promise`<`Transaction`<`InitiateEvent`\>\>

#### Overrides

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[findInitiateSwapTransaction](chainify_evm.EvmBaseSwapProvider.md#findinitiateswaptransaction)

#### Defined in

[evm/lib/swap/EvmSwapProvider.ts:16](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmSwapProvider.ts#L16)

___

### findRefundSwapTransaction

▸ **findRefundSwapTransaction**(`swapParams`, `initTxHash`): `Promise`<`Transaction`<`RefundEvent`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTxHash` | `string` |

#### Returns

`Promise`<`Transaction`<`RefundEvent`\>\>

#### Overrides

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[findRefundSwapTransaction](chainify_evm.EvmBaseSwapProvider.md#findrefundswaptransaction)

#### Defined in

[evm/lib/swap/EvmSwapProvider.ts:44](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmSwapProvider.ts#L44)

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

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[generateSecret](chainify_evm.EvmBaseSwapProvider.md#generatesecret)

#### Defined in

client/dist/lib/Swap.d.ts:10

___

### getSwapSecret

▸ **getSwapSecret**(`claimTx`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `claimTx` | `string` |

#### Returns

`Promise`<`string`\>

#### Inherited from

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[getSwapSecret](chainify_evm.EvmBaseSwapProvider.md#getswapsecret)

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:102](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L102)

___

### getWallet

▸ **getWallet**(): [`EvmBaseWalletProvider`](chainify_evm.EvmBaseWalletProvider.md)<`BaseProvider`, `Signer`\>

#### Returns

[`EvmBaseWalletProvider`](chainify_evm.EvmBaseWalletProvider.md)<`BaseProvider`, `Signer`\>

#### Inherited from

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[getWallet](chainify_evm.EvmBaseSwapProvider.md#getwallet)

#### Defined in

client/dist/lib/Swap.d.ts:7

___

### initiateSwap

▸ **initiateSwap**(`swapParams`, `fee`): `Promise`<`Transaction`<`TransactionResponse`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `fee` | `FeeType` |

#### Returns

`Promise`<`Transaction`<`TransactionResponse`\>\>

#### Inherited from

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[initiateSwap](chainify_evm.EvmBaseSwapProvider.md#initiateswap)

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:35](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L35)

___

### onWalletProviderUpdate

▸ `Protected` **onWalletProviderUpdate**(`wallet`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `wallet` | [`EvmBaseWalletProvider`](chainify_evm.EvmBaseWalletProvider.md)<`BaseProvider`, `Signer`\> |

#### Returns

`void`

#### Inherited from

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[onWalletProviderUpdate](chainify_evm.EvmBaseSwapProvider.md#onwalletproviderupdate)

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:127](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L127)

___

### refundSwap

▸ **refundSwap**(`swapParams`, `initTxHash`, `fee`): `Promise`<`Transaction`<`TransactionResponse`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTxHash` | `string` |
| `fee` | `FeeType` |

#### Returns

`Promise`<`Transaction`<`TransactionResponse`\>\>

#### Inherited from

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[refundSwap](chainify_evm.EvmBaseSwapProvider.md#refundswap)

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:78](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L78)

___

### setWallet

▸ **setWallet**(`wallet`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `wallet` | [`EvmBaseWalletProvider`](chainify_evm.EvmBaseWalletProvider.md)<`BaseProvider`, `Signer`\> |

#### Returns

`void`

#### Inherited from

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[setWallet](chainify_evm.EvmBaseSwapProvider.md#setwallet)

#### Defined in

client/dist/lib/Swap.d.ts:6

___

### tryParseLog

▸ `Protected` **tryParseLog**(`log`): `LogDescription`

#### Parameters

| Name | Type |
| :------ | :------ |
| `log` | `Log` |

#### Returns

`LogDescription`

#### Inherited from

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[tryParseLog](chainify_evm.EvmBaseSwapProvider.md#tryparselog)

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:157](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L157)

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

#### Inherited from

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[updateTransactionFee](chainify_evm.EvmBaseSwapProvider.md#updatetransactionfee)

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:123](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L123)

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

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[validateSwapParams](chainify_evm.EvmBaseSwapProvider.md#validateswapparams)

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

[EvmBaseSwapProvider](chainify_evm.EvmBaseSwapProvider.md).[verifyInitiateSwapTransaction](chainify_evm.EvmBaseSwapProvider.md#verifyinitiateswaptransaction)

#### Defined in

client/dist/lib/Swap.d.ts:8
