---
id: "chainify_evm.EvmTypes.SignTypedMessageType"
title: "Interface: SignTypedMessageType<V, T>"
sidebar_label: "SignTypedMessageType"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[EvmTypes](../namespaces/chainify_evm.EvmTypes.md).SignTypedMessageType

## Type parameters

| Name | Type |
| :------ | :------ |
| `V` | extends `SignTypedDataVersion` = `SignTypedDataVersion` |
| `T` | extends `MessageTypes` = `MessageTypes` |

## Properties

### data

• **data**: `V` extends ``"V1"`` ? `TypedDataV1` : `TypedMessage`<`T`\>

#### Defined in

[evm/lib/types.ts:9](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/types.ts#L9)

___

### from

• **from**: `string`

#### Defined in

[evm/lib/types.ts:11](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/types.ts#L11)

___

### version

• **version**: `SignTypedDataVersion`

#### Defined in

[evm/lib/types.ts:10](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/types.ts#L10)
