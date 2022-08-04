---
id: "chainify_evm.RpcFeeProvider"
title: "Class: RpcFeeProvider"
sidebar_label: "RpcFeeProvider"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).RpcFeeProvider

## Hierarchy

- `default`

  ↳ **`RpcFeeProvider`**

## Constructors

### constructor

• **new RpcFeeProvider**(`provider`, `feeOptions?`, `network?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `provider` | `string` \| `StaticJsonRpcProvider` |
| `feeOptions?` | [`FeeOptions`](../namespaces/chainify_evm.EvmTypes.md#feeoptions) |
| `network?` | `Network` |

#### Overrides

Fee.constructor

#### Defined in

[evm/lib/fee/RpcFeeProvider.ts:11](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/fee/RpcFeeProvider.ts#L11)

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

[evm/lib/fee/RpcFeeProvider.ts:27](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/fee/RpcFeeProvider.ts#L27)
