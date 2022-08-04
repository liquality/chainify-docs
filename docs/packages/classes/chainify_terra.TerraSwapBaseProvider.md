---
id: "chainify_terra.TerraSwapBaseProvider"
title: "Class: TerraSwapBaseProvider"
sidebar_label: "TerraSwapBaseProvider"
custom_edit_url: null
---

[@chainify/terra](../modules/chainify_terra.md).TerraSwapBaseProvider

## Hierarchy

- `default`<`LCDClient`, `MnemonicKey`, [`TerraWalletProvider`](chainify_terra.TerraWalletProvider.md)\>

  ↳ **`TerraSwapBaseProvider`**

  ↳↳ [`TerraSwapProvider`](chainify_terra.TerraSwapProvider.md)

## Constructors

### constructor

• **new TerraSwapBaseProvider**(`walletProvider?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `walletProvider?` | [`TerraWalletProvider`](chainify_terra.TerraWalletProvider.md) |

#### Inherited from

Swap<LCDClient, MnemonicKey, TerraWalletProvider\>.constructor

#### Defined in

client/dist/lib/Swap.d.ts:5

## Properties

### walletProvider

• `Protected` **walletProvider**: [`TerraWalletProvider`](chainify_terra.TerraWalletProvider.md)

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

#### Overrides

Swap.claimSwap

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

#### Overrides

Swap.doesTransactionMatchInitiation

#### Defined in

[terra/lib/swap/TerraSwapBaseProvider.ts:73](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapBaseProvider.ts#L73)

___

### findClaimSwapTransaction

▸ `Abstract` **findClaimSwapTransaction**(`_swapParams`, `_initTxHash`, `_blockNumber?`): `Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_swapParams` | `SwapParams` |
| `_initTxHash` | `string` |
| `_blockNumber?` | `number` |

#### Returns

`Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Overrides

Swap.findClaimSwapTransaction

#### Defined in

[terra/lib/swap/TerraSwapBaseProvider.ts:97](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapBaseProvider.ts#L97)

___

### findInitiateSwapTransaction

▸ `Abstract` **findInitiateSwapTransaction**(`_swapParams`, `_blockNumber?`): `Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_swapParams` | `SwapParams` |
| `_blockNumber?` | `number` |

#### Returns

`Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Overrides

Swap.findInitiateSwapTransaction

#### Defined in

[terra/lib/swap/TerraSwapBaseProvider.ts:95](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapBaseProvider.ts#L95)

___

### findRefundSwapTransaction

▸ `Abstract` **findRefundSwapTransaction**(`_swapParams`, `_initiationTxHash`, `_blockNumber?`): `Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_swapParams` | `SwapParams` |
| `_initiationTxHash` | `string` |
| `_blockNumber?` | `number` |

#### Returns

`Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Overrides

Swap.findRefundSwapTransaction

#### Defined in

[terra/lib/swap/TerraSwapBaseProvider.ts:103](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapBaseProvider.ts#L103)

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

▸ **getSwapSecret**(`claimTxHash`, `_initTxHash?`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `claimTxHash` | `string` |
| `_initTxHash?` | `string` |

#### Returns

`Promise`<`string`\>

#### Overrides

Swap.getSwapSecret

#### Defined in

[terra/lib/swap/TerraSwapBaseProvider.ts:68](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapBaseProvider.ts#L68)

___

### getWallet

▸ **getWallet**(): [`TerraWalletProvider`](chainify_terra.TerraWalletProvider.md)

#### Returns

[`TerraWalletProvider`](chainify_terra.TerraWalletProvider.md)

#### Inherited from

Swap.getWallet

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

#### Overrides

Swap.initiateSwap

#### Defined in

[terra/lib/swap/TerraSwapBaseProvider.ts:11](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/swap/TerraSwapBaseProvider.ts#L11)

___

### onWalletProviderUpdate

▸ `Protected` `Abstract` **onWalletProviderUpdate**(`wallet`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `wallet` | [`TerraWalletProvider`](chainify_terra.TerraWalletProvider.md) |

#### Returns

`void`

#### Inherited from

Swap.onWalletProviderUpdate

#### Defined in

client/dist/lib/Swap.d.ts:21

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

#### Overrides

Swap.refundSwap

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

Swap.setWallet

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

#### Overrides

Swap.updateTransactionFee

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
