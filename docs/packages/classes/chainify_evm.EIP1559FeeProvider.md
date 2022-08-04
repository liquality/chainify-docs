---
id: "chainify_evm.EIP1559FeeProvider"
title: "Class: EIP1559FeeProvider"
sidebar_label: "EIP1559FeeProvider"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).EIP1559FeeProvider

## Hierarchy

- `default`

  ↳ **`EIP1559FeeProvider`**

## Constructors

### constructor

• **new EIP1559FeeProvider**(`provider`, `network?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `provider` | `string` \| `StaticJsonRpcProvider` |
| `network?` | `Network` |

#### Overrides

Fee.constructor

#### Defined in

[evm/lib/fee/EIP1559FeeProvider.ts:10](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/fee/EIP1559FeeProvider.ts#L10)

## Properties

### gasUnits

• **gasUnits**: `BigNumber`

#### Inherited from

Fee.gasUnits

#### Defined in

client/dist/lib/Fee.d.ts:3

___

### provider

• **provider**: `StaticJsonRpcProvider`

#### Defined in

[evm/lib/fee/EIP1559FeeProvider.ts:8](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/fee/EIP1559FeeProvider.ts#L8)

## Methods

### calculateMaxFeePerGas

▸ **calculateMaxFeePerGas**(`maxPriorityFeePerGas`, `potentialMaxFee`): `BigNumber`

#### Parameters

| Name | Type |
| :------ | :------ |
| `maxPriorityFeePerGas` | `BigNumber` |
| `potentialMaxFee` | `BigNumber` |

#### Returns

`BigNumber`

#### Defined in

[evm/lib/fee/EIP1559FeeProvider.ts:33](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/fee/EIP1559FeeProvider.ts#L33)

___

### getBaseFeeMultiplier

▸ **getBaseFeeMultiplier**(`baseFeeTrend`): ``1.6`` \| ``1.4`` \| ``1.2`` \| ``1.1``

#### Parameters

| Name | Type |
| :------ | :------ |
| `baseFeeTrend` | `number` |

#### Returns

``1.6`` \| ``1.4`` \| ``1.2`` \| ``1.1``

#### Defined in

[evm/lib/fee/EIP1559FeeProvider.ts:20](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/fee/EIP1559FeeProvider.ts#L20)

___

### getFees

▸ **getFees**(): `Promise`<`FeeDetails`\>

#### Returns

`Promise`<`FeeDetails`\>

#### Overrides

Fee.getFees

#### Defined in

[evm/lib/fee/EIP1559FeeProvider.ts:37](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/fee/EIP1559FeeProvider.ts#L37)
