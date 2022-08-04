---
id: "chainify_evm.EnsProvider"
title: "Class: EnsProvider"
sidebar_label: "EnsProvider"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).EnsProvider

## Implements

- `NamingProvider`

## Constructors

### constructor

• **new EnsProvider**(`provider`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `provider` | `StaticJsonRpcProvider` |

#### Defined in

[evm/lib/naming/EnsProvider.ts:7](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/naming/EnsProvider.ts#L7)

## Methods

### lookupAddress

▸ **lookupAddress**(`address`): `Promise`<`string`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `address` | `AddressType` |  |

#### Returns

`Promise`<`string`\>

#### Implementation of

NamingProvider.lookupAddress

#### Defined in

[evm/lib/naming/EnsProvider.ts:23](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/naming/EnsProvider.ts#L23)

___

### resolveName

▸ **resolveName**(`name`): `Promise`<`AddressType`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |

#### Returns

`Promise`<`AddressType`\>

#### Implementation of

NamingProvider.resolveName

#### Defined in

[evm/lib/naming/EnsProvider.ts:15](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/naming/EnsProvider.ts#L15)
