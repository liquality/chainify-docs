---
id: "chainify_near.NearTypes.NearAccount"
title: "Class: NearAccount"
sidebar_label: "NearAccount"
custom_edit_url: null
---

[@chainify/near](../modules/chainify_near.md).[NearTypes](../namespaces/chainify_near.NearTypes.md).NearAccount

## Hierarchy

- `Account`

  ↳ **`NearAccount`**

## Constructors

### constructor

• **new NearAccount**(`connection`, `accountId`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `connection` | `Connection` |
| `accountId` | `string` |

#### Overrides

Account.constructor

#### Defined in

[near/lib/types.ts:79](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/types.ts#L79)

## Methods

### signAndSendTransaction

▸ **signAndSendTransaction**(`__namedParameters`): `Promise`<`FinalExecutionOutcome`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters` | `any` |

#### Returns

`Promise`<`FinalExecutionOutcome`\>

#### Overrides

Account.signAndSendTransaction

#### Defined in

[near/lib/types.ts:82](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/types.ts#L82)
