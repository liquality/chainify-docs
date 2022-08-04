---
id: "chainify_evm.EvmBaseSwapProvider"
title: "Class: EvmBaseSwapProvider"
sidebar_label: "EvmBaseSwapProvider"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).EvmBaseSwapProvider

## Hierarchy

- `default`<`BaseProvider`, `Signer`, [`EvmBaseWalletProvider`](chainify_evm.EvmBaseWalletProvider.md)<`BaseProvider`\>\>

  ↳ **`EvmBaseSwapProvider`**

  ↳↳ [`EvmSwapProvider`](chainify_evm.EvmSwapProvider.md)

## Constructors

### constructor

• **new EvmBaseSwapProvider**(`swapOptions?`, `walletProvider?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapOptions?` | [`EvmSwapOptions`](../interfaces/chainify_evm.EvmTypes.EvmSwapOptions.md) |
| `walletProvider?` | [`EvmBaseWalletProvider`](chainify_evm.EvmBaseWalletProvider.md)<`BaseProvider`, `Signer`\> |

#### Overrides

Swap&lt;BaseProvider, Signer, EvmBaseWalletProvider&lt;BaseProvider\&gt;\&gt;.constructor

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:19](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L19)

## Properties

### contract

• `Protected` **contract**: [`LiqualityHTLC`](../interfaces/chainify_evm.Typechain.LiqualityHTLC.md)

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:16](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L16)

___

### swapOptions

• `Protected` **swapOptions**: [`EvmSwapOptions`](../interfaces/chainify_evm.EvmTypes.EvmSwapOptions.md)

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:17](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L17)

___

### walletProvider

• `Protected` **walletProvider**: [`EvmBaseWalletProvider`](chainify_evm.EvmBaseWalletProvider.md)<`BaseProvider`, `Signer`\>

#### Overrides

Swap.walletProvider

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:15](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L15)

## Methods

### canUpdateFee

▸ **canUpdateFee**(): `boolean`

#### Returns

`boolean`

#### Overrides

Swap.canUpdateFee

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

#### Overrides

Swap.claimSwap

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

#### Overrides

Swap.doesTransactionMatchInitiation

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:131](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L131)

___

### findClaimSwapTransaction

▸ `Abstract` **findClaimSwapTransaction**(`swapParams`, `initTxHash`, `_blockNumber?`): `Promise`<`Transaction`<`ClaimEvent`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTxHash` | `string` |
| `_blockNumber?` | `number` |

#### Returns

`Promise`<`Transaction`<`ClaimEvent`\>\>

#### Overrides

Swap.findClaimSwapTransaction

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:173](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L173)

___

### findInitiateSwapTransaction

▸ `Abstract` **findInitiateSwapTransaction**(`swapParams`, `_blockNumber?`): `Promise`<`Transaction`<`InitiateEvent`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `_blockNumber?` | `number` |

#### Returns

`Promise`<`Transaction`<`InitiateEvent`\>\>

#### Overrides

Swap.findInitiateSwapTransaction

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:169](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L169)

___

### findRefundSwapTransaction

▸ `Abstract` **findRefundSwapTransaction**(`swapParams`, `initTxHash`, `blockNumber?`): `Promise`<`Transaction`<`RefundEvent`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `swapParams` | `SwapParams` |
| `initTxHash` | `string` |
| `blockNumber?` | `number` |

#### Returns

`Promise`<`Transaction`<`RefundEvent`\>\>

#### Overrides

Swap.findRefundSwapTransaction

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:171](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L171)

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

▸ **getSwapSecret**(`claimTx`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `claimTx` | `string` |

#### Returns

`Promise`<`string`\>

#### Overrides

Swap.getSwapSecret

#### Defined in

[evm/lib/swap/EvmBaseSwapProvider.ts:102](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/swap/EvmBaseSwapProvider.ts#L102)

___

### getWallet

▸ **getWallet**(): [`EvmBaseWalletProvider`](chainify_evm.EvmBaseWalletProvider.md)<`BaseProvider`, `Signer`\>

#### Returns

[`EvmBaseWalletProvider`](chainify_evm.EvmBaseWalletProvider.md)<`BaseProvider`, `Signer`\>

#### Inherited from

Swap.getWallet

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

#### Overrides

Swap.initiateSwap

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

#### Overrides

Swap.onWalletProviderUpdate

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

#### Overrides

Swap.refundSwap

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

Swap.setWallet

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

#### Overrides

Swap.updateTransactionFee

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
