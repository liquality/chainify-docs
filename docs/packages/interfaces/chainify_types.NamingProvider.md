---
id: "chainify_types.NamingProvider"
title: "Interface: NamingProvider"
sidebar_label: "NamingProvider"
custom_edit_url: null
---

[@chainify/types](../modules/chainify_types.md).NamingProvider

## Methods

### lookupAddress

▸ **lookupAddress**(`address`): `Promise`<`string`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `address` | [`AddressType`](../modules/chainify_types.md#addresstype) |  |

#### Returns

`Promise`<`string`\>

#### Defined in

[types/lib/Naming.ts:14](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Naming.ts#L14)

___

### resolveName

▸ **resolveName**(`name`): `Promise`<[`AddressType`](../modules/chainify_types.md#addresstype)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |

#### Returns

`Promise`<[`AddressType`](../modules/chainify_types.md#addresstype)\>

#### Defined in

[types/lib/Naming.ts:8](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Naming.ts#L8)
