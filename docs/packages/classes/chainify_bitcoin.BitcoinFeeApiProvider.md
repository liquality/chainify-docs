---
id: "chainify_bitcoin.BitcoinFeeApiProvider"
title: "Class: BitcoinFeeApiProvider"
sidebar_label: "BitcoinFeeApiProvider"
custom_edit_url: null
---

[@chainify/bitcoin](../modules/chainify_bitcoin.md).BitcoinFeeApiProvider

## Hierarchy

- `default`

  ↳ **`BitcoinFeeApiProvider`**

## Implements

- `FeeProvider`

## Constructors

### constructor

• **new BitcoinFeeApiProvider**(`endpoint?`)

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `endpoint` | `string` | `'https://mempool.space/api/v1/fees/recommended'` |

#### Overrides

Fee.constructor

#### Defined in

[bitcoin/lib/fee/BitcoinFeeApiProvider.ts:7](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/fee/BitcoinFeeApiProvider.ts#L7)

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

#### Implementation of

FeeProvider.getFees

#### Overrides

Fee.getFees

#### Defined in

[bitcoin/lib/fee/BitcoinFeeApiProvider.ts:12](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/fee/BitcoinFeeApiProvider.ts#L12)
