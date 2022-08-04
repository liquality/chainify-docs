---
id: "chainify_client.HttpClient"
title: "Class: HttpClient"
sidebar_label: "HttpClient"
custom_edit_url: null
---

[@chainify/client](../modules/chainify_client.md).HttpClient

## Constructors

### constructor

• **new HttpClient**(`config`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `config` | `AxiosRequestConfig`<`any`\> |

#### Defined in

[client/lib/Http.ts:9](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Http.ts#L9)

## Methods

### nodeGet

▸ **nodeGet**<`I`, `O`\>(`url`, `params?`, `config?`): `Promise`<`O`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `I` | `any` |
| `O` | `any` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |
| `params` | `I` |
| `config?` | `AxiosRequestConfig`<`any`\> |

#### Returns

`Promise`<`O`\>

#### Defined in

[client/lib/Http.ts:31](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Http.ts#L31)

___

### nodePost

▸ **nodePost**<`I`, `O`\>(`url`, `data`, `config?`): `Promise`<`O`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `I` | `any` |
| `O` | `any` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |
| `data` | `I` |
| `config?` | `AxiosRequestConfig`<`any`\> |

#### Returns

`Promise`<`O`\>

#### Defined in

[client/lib/Http.ts:40](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Http.ts#L40)

___

### setConfig

▸ **setConfig**(`config`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `config` | `AxiosRequestConfig`<`any`\> |

#### Returns

`void`

#### Defined in

[client/lib/Http.ts:49](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Http.ts#L49)

___

### get

▸ `Static` **get**<`I`, `O`\>(`url`, `params?`, `config?`): `Promise`<`O`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `I` | `any` |
| `O` | `any` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |
| `params` | `I` |
| `config?` | `AxiosRequestConfig`<`any`\> |

#### Returns

`Promise`<`O`\>

#### Defined in

[client/lib/Http.ts:22](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Http.ts#L22)

___

### post

▸ `Static` **post**<`I`, `O`\>(`url`, `data`, `config?`): `Promise`<`O`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `I` | `any` |
| `O` | `any` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `url` | `string` |
| `data` | `I` |
| `config?` | `AxiosRequestConfig`<`any`\> |

#### Returns

`Promise`<`O`\>

#### Defined in

[client/lib/Http.ts:13](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Http.ts#L13)
