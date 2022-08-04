---
id: "chainify_client.Fee"
title: "Class: Fee"
sidebar_label: "Fee"
custom_edit_url: null
---

[@chainify/client](../modules/chainify_client.md).Fee

## Implements

- `FeeProvider`

## Constructors

### constructor

• **new Fee**(`gasUnits?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `gasUnits?` | `BigNumber` |

#### Defined in

[client/lib/Fee.ts:6](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Fee.ts#L6)

## Properties

### gasUnits

• **gasUnits**: `BigNumber`

#### Defined in

[client/lib/Fee.ts:4](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Fee.ts#L4)

## Methods

### getFees

▸ `Abstract` **getFees**(`feeAsset?`): `Promise`<`FeeDetails`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `feeAsset?` | `Asset` |

#### Returns

`Promise`<`FeeDetails`\>

#### Implementation of

FeeProvider.getFees

#### Defined in

[client/lib/Fee.ts:10](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Fee.ts#L10)
