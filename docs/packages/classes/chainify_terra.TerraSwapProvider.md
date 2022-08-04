---
id: "chainify_terra.TerraSwapProvider"
title: "Class: TerraSwapProvider"
sidebar_label: "TerraSwapProvider"
custom_edit_url: null
---

[@chainify/terra](../modules/chainify_terra.md).TerraSwapProvider

## Hierarchy

- [`TerraSwapBaseProvider`](chainify_terra.TerraSwapBaseProvider.md)

  ↳ **`TerraSwapProvider`**

## Constructors

### constructor

• **new TerraSwapProvider**(`helperUrl`, `walletProvider?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `helperUrl` | `string` |
| `walletProvider?` | [`TerraWalletProvider`](chainify_terra.TerraWalletProvider.md) |

#### Overrides

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[constructor](chainify_terra.TerraSwapBaseProvider.md#constructor)

#### Defined in

[terra/lib/swap/TerraSwapProvider.ts:19](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapProvider.ts#L19)

## Properties

### walletProvider

• `Protected` **walletProvider**: [`TerraWalletProvider`](chainify_terra.TerraWalletProvider.md)

#### Inherited from

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[walletProvider](chainify_terra.TerraSwapBaseProvider.md#walletprovider)

#### Defined in

client/dist/lib/Swap.d.ts:4

## Methods

### canUpdateFee

▸ **canUpdateFee**(): `boolean`

#### Returns

`boolean`

#### Inherited from

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[canUpdateFee](chainify_terra.TerraSwapBaseProvider.md#canupdatefee)

#### Defined in

[terra/lib/swap/TerraSwapBaseProvider.ts:87](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapBaseProvider.ts#L87)

___

### claimSwap

▸ **claimSwap**(`swapParams`, `initiationTxHash`, `secret`, `fee?`): `Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initiationTxHash` | `string` |
| `secret` | `string` |
| `fee?` | `FeeType` |

#### Returns

`Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Inherited from

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[claimSwap](chainify_terra.TerraSwapBaseProvider.md#claimswap)

#### Defined in

[terra/lib/swap/TerraSwapBaseProvider.ts:42](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapBaseProvider.ts#L42)

___

### doesTransactionMatchInitiation

▸ `Protected` **doesTransactionMatchInitiation**(`swapParams`, `initTx`): `Promise`<`boolean`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTx` | `Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\> |

#### Returns

`Promise`<`boolean`\>

#### Inherited from

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[doesTransactionMatchInitiation](chainify_terra.TerraSwapBaseProvider.md#doestransactionmatchinitiation)

#### Defined in

[terra/lib/swap/TerraSwapBaseProvider.ts:73](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapBaseProvider.ts#L73)

___

### findClaimSwapTransaction

▸ **findClaimSwapTransaction**(`swapParams`, `initTxHash`): `Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTxHash` | `string` |

#### Returns

`Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Overrides

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[findClaimSwapTransaction](chainify_terra.TerraSwapBaseProvider.md#findclaimswaptransaction)

#### Defined in

[terra/lib/swap/TerraSwapProvider.ts:33](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapProvider.ts#L33)

___

### findInitiateSwapTransaction

▸ **findInitiateSwapTransaction**(`swapParams`): `Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |

#### Returns

`Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Overrides

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[findInitiateSwapTransaction](chainify_terra.TerraSwapBaseProvider.md#findinitiateswaptransaction)

#### Defined in

[terra/lib/swap/TerraSwapProvider.ts:24](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapProvider.ts#L24)

___

### findRefundSwapTransaction

▸ **findRefundSwapTransaction**(`swapParams`, `initTxHash`): `Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTxHash` | `string` |

#### Returns

`Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Overrides

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[findRefundSwapTransaction](chainify_terra.TerraSwapBaseProvider.md#findrefundswaptransaction)

#### Defined in

[terra/lib/swap/TerraSwapProvider.ts:45](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapProvider.ts#L45)

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

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[generateSecret](chainify_terra.TerraSwapBaseProvider.md#generatesecret)

#### Defined in

client/dist/lib/Swap.d.ts:10

___

### getSwapSecret

▸ **getSwapSecret**(`claimTxHash`, `_initTxHash?`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `claimTxHash` | `string` |
| `_initTxHash?` | `string` |

#### Returns

`Promise`<`string`\>

#### Inherited from

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[getSwapSecret](chainify_terra.TerraSwapBaseProvider.md#getswapsecret)

#### Defined in

[terra/lib/swap/TerraSwapBaseProvider.ts:68](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapBaseProvider.ts#L68)

___

### getWallet

▸ **getWallet**(): [`TerraWalletProvider`](chainify_terra.TerraWalletProvider.md)

#### Returns

[`TerraWalletProvider`](chainify_terra.TerraWalletProvider.md)

#### Inherited from

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[getWallet](chainify_terra.TerraSwapBaseProvider.md#getwallet)

#### Defined in

client/dist/lib/Swap.d.ts:7

___

### initiateSwap

▸ **initiateSwap**(`swapParams`, `fee?`): `Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `fee?` | `FeeType` |

#### Returns

`Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Inherited from

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[initiateSwap](chainify_terra.TerraSwapBaseProvider.md#initiateswap)

#### Defined in

[terra/lib/swap/TerraSwapBaseProvider.ts:11](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapBaseProvider.ts#L11)

___

### onWalletProviderUpdate

▸ `Protected` **onWalletProviderUpdate**(`_wallet`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `_wallet` | [`TerraWalletProvider`](chainify_terra.TerraWalletProvider.md) |

#### Returns

`void`

#### Overrides

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[onWalletProviderUpdate](chainify_terra.TerraSwapBaseProvider.md#onwalletproviderupdate)

#### Defined in

[terra/lib/swap/TerraSwapProvider.ts:56](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapProvider.ts#L56)

___

### refundSwap

▸ **refundSwap**(`swapParams`, `initTx`, `fee?`): `Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTx` | `string` |
| `fee?` | `FeeType` |

#### Returns

`Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Inherited from

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[refundSwap](chainify_terra.TerraSwapBaseProvider.md#refundswap)

#### Defined in

[terra/lib/swap/TerraSwapBaseProvider.ts:59](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapBaseProvider.ts#L59)

___

### setWallet

▸ **setWallet**(`wallet`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `wallet` | [`TerraWalletProvider`](chainify_terra.TerraWalletProvider.md) |

#### Returns

`void`

#### Inherited from

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[setWallet](chainify_terra.TerraSwapBaseProvider.md#setwallet)

#### Defined in

client/dist/lib/Swap.d.ts:6

___

### updateTransactionFee

▸ **updateTransactionFee**(`_tx`, `_newFee`): `Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_tx` | `string` \| `Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\> |
| `_newFee` | `FeeType` |

#### Returns

`Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Inherited from

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[updateTransactionFee](chainify_terra.TerraSwapBaseProvider.md#updatetransactionfee)

#### Defined in

[terra/lib/swap/TerraSwapBaseProvider.ts:91](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapBaseProvider.ts#L91)

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

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[validateSwapParams](chainify_terra.TerraSwapBaseProvider.md#validateswapparams)

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

[TerraSwapBaseProvider](chainify_terra.TerraSwapBaseProvider.md).[verifyInitiateSwapTransaction](chainify_terra.TerraSwapBaseProvider.md#verifyinitiateswaptransaction)

#### Defined in

client/dist/lib/Swap.d.ts:8
