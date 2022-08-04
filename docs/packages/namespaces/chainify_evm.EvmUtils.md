---
id: "chainify_evm.EvmUtils"
title: "Namespace: EvmUtils"
sidebar_label: "EvmUtils"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).EvmUtils

## Functions

### calculateFee

▸ **calculateFee**(`base`, `multiplier`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `base` | `string` \| `number` \| `BigNumber` |
| `multiplier` | `number` |

#### Returns

`number`

#### Defined in

[evm/lib/utils.ts:145](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/utils.ts#L145)

___

### calculateGasMargin

▸ **calculateGasMargin**(`value`, `margin?`): `BigNumber`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `value` | `BigNumberish` | `undefined` |
| `margin` | `number` | `1000` |

#### Returns

`BigNumber`

#### Defined in

[evm/lib/utils.ts:155](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/utils.ts#L155)

___

### extractFeeData

▸ **extractFeeData**(`fee`): { `gasPrice`: `number`  } \| { `baseFeeTrend?`: `number` ; `currentBaseFeePerGas?`: `number` ; `gasPrice`: `undefined` ; `maxFeePerGas`: `number` ; `maxPriorityFeePerGas`: `number` ; `suggestedBaseFeePerGas?`: `number`  }

#### Parameters

| Name | Type |
| :------ | :------ |
| `fee` | `FeeType` |

#### Returns

{ `gasPrice`: `number`  } \| { `baseFeeTrend?`: `number` ; `currentBaseFeePerGas?`: `number` ; `gasPrice`: `undefined` ; `maxFeePerGas`: `number` ; `maxPriorityFeePerGas`: `number` ; `suggestedBaseFeePerGas?`: `number`  }

#### Defined in

[evm/lib/utils.ts:120](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/utils.ts#L120)

___

### fromGwei

▸ **fromGwei**(`gwei`): `BigNumber`

#### Parameters

| Name | Type |
| :------ | :------ |
| `gwei` | `string` \| `number` \| `BigNumber` |

#### Returns

`BigNumber`

#### Defined in

[evm/lib/utils.ts:141](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/utils.ts#L141)

___

### generateId

▸ **generateId**(`htlcData`, `blockTimestamp`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `htlcData` | [`HTLCDataStruct`](chainify_evm.Typechain.ILiqualityHTLC.md#htlcdatastruct) |
| `blockTimestamp` | `number` |

#### Returns

`string`

#### Defined in

[evm/lib/utils.ts:106](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/utils.ts#L106)

___

### parseBlockResponse

▸ **parseBlockResponse**(`block`, `transactions?`): `Block`<`EthersBlock` \| `EthersBlockWithTransactions`, `EthersTransactionResponse`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `block` | `Block` \| `BlockWithTransactions` |
| `transactions?` | `TransactionResponse`[] |

#### Returns

`Block`<`EthersBlock` \| `EthersBlockWithTransactions`, `EthersTransactionResponse`\>

#### Defined in

[evm/lib/utils.ts:90](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/utils.ts#L90)

___

### parseSwapParams

▸ **parseSwapParams**(`tx`): [`HTLCDataStruct`](chainify_evm.Typechain.ILiqualityHTLC.md#htlcdatastruct)

#### Parameters

| Name | Type |
| :------ | :------ |
| `tx` | `SwapParams` |

#### Returns

[`HTLCDataStruct`](chainify_evm.Typechain.ILiqualityHTLC.md#htlcdatastruct)

#### Defined in

[evm/lib/utils.ts:29](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/utils.ts#L29)

___

### parseTxRequest

▸ **parseTxRequest**(`request`): `TransactionRequest`

#### Parameters

| Name | Type |
| :------ | :------ |
| `request` | `TransactionRequest` \| [`EthereumTransactionRequest`](chainify_evm.EvmTypes.md#ethereumtransactionrequest) |

#### Returns

`TransactionRequest`

#### Defined in

[evm/lib/utils.ts:40](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/utils.ts#L40)

___

### parseTxResponse

▸ **parseTxResponse**(`response`, `receipt?`): `Transaction`<`EthersTransactionResponse`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `response` | `TransactionResponse` |
| `receipt?` | `TransactionReceipt` |

#### Returns

`Transaction`<`EthersTransactionResponse`\>

#### Defined in

[evm/lib/utils.ts:66](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/utils.ts#L66)

___

### toEthereumTxRequest

▸ **toEthereumTxRequest**(`tx`, `fee`): [`EthereumTransactionRequest`](chainify_evm.EvmTypes.md#ethereumtransactionrequest)

#### Parameters

| Name | Type |
| :------ | :------ |
| `tx` | `PopulatedTransaction` |
| `fee` | `FeeType` |

#### Returns

[`EthereumTransactionRequest`](chainify_evm.EvmTypes.md#ethereumtransactionrequest)

#### Defined in

[evm/lib/utils.ts:17](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/utils.ts#L17)

___

### toGwei

▸ **toGwei**(`wei`): `BigNumber`

#### Parameters

| Name | Type |
| :------ | :------ |
| `wei` | `string` \| `number` \| `BigNumber` |

#### Returns

`BigNumber`

#### Defined in

[evm/lib/utils.ts:137](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/utils.ts#L137)
