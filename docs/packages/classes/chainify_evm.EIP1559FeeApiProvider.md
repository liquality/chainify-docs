---
id: "chainify_evm.EIP1559FeeApiProvider"
title: "Class: EIP1559FeeApiProvider"
sidebar_label: "EIP1559FeeApiProvider"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).EIP1559FeeApiProvider

## Hierarchy

- `default`

  ↳ **`EIP1559FeeApiProvider`**

## Constructors

### constructor

• **new EIP1559FeeApiProvider**(`url`, `chainId`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |
| `chainId` | `number` |

#### Overrides

Fee.constructor

#### Defined in

[evm/lib/fee/EIP1559FeeApiProvider/index.ts:12](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/fee/EIP1559FeeApiProvider/index.ts#L12)

## Properties

### gasUnits

• **gasUnits**: `BigNumber`

#### Inherited from

Fee.gasUnits

#### Defined in

client/dist/lib/Fee.d.ts:3

## Methods

### getFees

▸ **getFees**(): `Promise`<`FeeDetails`\>

#### Returns

`Promise`<`FeeDetails`\>

#### Overrides

Fee.getFees

#### Defined in

[evm/lib/fee/EIP1559FeeApiProvider/index.ts:18](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/fee/EIP1559FeeApiProvider/index.ts#L18)
