---
id: "chainify_client.JsonRpcProvider"
title: "Class: JsonRpcProvider"
sidebar_label: "JsonRpcProvider"
custom_edit_url: null
---

[@chainify/client](../modules/chainify_client.md).JsonRpcProvider

## Constructors

### constructor

• **new JsonRpcProvider**(`url?`, `username?`, `password?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `url?` | `string` |
| `username?` | `string` |
| `password?` | `string` |

#### Defined in

[client/lib/JsonRpc.ts:11](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/JsonRpc.ts#L11)

## Methods

### send

▸ **send**(`method`, `params`): `Promise`<`any`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `method` | `string` |
| `params` | `any`[] |

#### Returns

`Promise`<`any`\>

#### Defined in

[client/lib/JsonRpc.ts:32](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/JsonRpc.ts#L32)

___

### defaultUrl

▸ `Static` **defaultUrl**(): `string`

#### Returns

`string`

#### Defined in

[client/lib/JsonRpc.ts:28](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/JsonRpc.ts#L28)
