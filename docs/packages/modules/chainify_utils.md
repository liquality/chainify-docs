---
id: "chainify_utils"
title: "Module: @chainify/utils"
sidebar_label: "@chainify/utils"
sidebar_position: 0
custom_edit_url: null
---

## Namespaces

- [Math](../namespaces/chainify_utils.Math.md)

## Functions

### asyncSetImmediate

▸ **asyncSetImmediate**(): `Promise`<`unknown`\>

#### Returns

`Promise`<`unknown`\>

#### Defined in

[utils/lib/index.ts:8](https://github.com/liquality/chainify/blob/540cfa69/packages/utils/lib/index.ts#L8)

___

### compare

▸ **compare**(`a`, `b`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `a` | `BigNumberish` |
| `b` | `BigNumberish` |

#### Returns

`boolean`

#### Defined in

[utils/lib/string.ts:3](https://github.com/liquality/chainify/blob/540cfa69/packages/utils/lib/string.ts#L3)

___

### ensure0x

▸ **ensure0x**(`hash`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `hash` | `string` |

#### Returns

`string`

#### Defined in

[utils/lib/hex.ts:4](https://github.com/liquality/chainify/blob/540cfa69/packages/utils/lib/hex.ts#L4)

___

### ensureBuffer

▸ **ensureBuffer**(`message`): ``false`` \| `Buffer`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `any` |  |

#### Returns

``false`` \| `Buffer`

#### Defined in

[utils/lib/crypto.ts:12](https://github.com/liquality/chainify/blob/540cfa69/packages/utils/lib/crypto.ts#L12)

___

### hash160

▸ **hash160**(`message`): `string`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` |  |

#### Returns

`string`

#### Defined in

[utils/lib/crypto.ts:32](https://github.com/liquality/chainify/blob/540cfa69/packages/utils/lib/crypto.ts#L32)

___

### isHex

▸ **isHex**(`hex`): `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `hex` | `string` |

#### Returns

`boolean`

#### Defined in

[utils/lib/crypto.ts:40](https://github.com/liquality/chainify/blob/540cfa69/packages/utils/lib/crypto.ts#L40)

___

### padHexStart

▸ **padHexStart**(`hex`, `lengthBytes?`): `string`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hex` | `string` |  |
| `lengthBytes?` | `number` |  |

#### Returns

`string`

#### Defined in

[utils/lib/crypto.ts:55](https://github.com/liquality/chainify/blob/540cfa69/packages/utils/lib/crypto.ts#L55)

___

### remove0x

▸ **remove0x**(`hash`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `hash` | `string` |

#### Returns

`string`

#### Defined in

[utils/lib/hex.ts:13](https://github.com/liquality/chainify/blob/540cfa69/packages/utils/lib/hex.ts#L13)

___

### retry

▸ **retry**<`T`\>(`method`, `startWaitTime?`, `waitBackoff?`, `retryNumber?`): `Promise`<`T`\>

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `method` | () => `Promise`<`T`\> | `undefined` |
| `startWaitTime` | `number` | `500` |
| `waitBackoff` | `number` | `2` |
| `retryNumber` | `number` | `5` |

#### Returns

`Promise`<`T`\>

#### Defined in

[utils/lib/index.ts:12](https://github.com/liquality/chainify/blob/540cfa69/packages/utils/lib/index.ts#L12)

___

### sha256

▸ **sha256**(`data`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | `string` |

#### Returns

`string`

#### Defined in

[utils/lib/crypto.ts:36](https://github.com/liquality/chainify/blob/540cfa69/packages/utils/lib/crypto.ts#L36)

___

### sleep

▸ **sleep**(`ms`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `ms` | `number` |

#### Returns

`Promise`<`void`\>

#### Defined in

[utils/lib/index.ts:33](https://github.com/liquality/chainify/blob/540cfa69/packages/utils/lib/index.ts#L33)

___

### toStringDeep

▸ **toStringDeep**<`I`, `O`\>(`input`): `O`

#### Type parameters

| Name |
| :------ |
| `I` |
| `O` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `input` | `I` |

#### Returns

`O`

#### Defined in

[utils/lib/string.ts:7](https://github.com/liquality/chainify/blob/540cfa69/packages/utils/lib/string.ts#L7)

___

### validateExpiration

▸ **validateExpiration**(`expiration`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `expiration` | `number` |

#### Returns

`void`

#### Defined in

[utils/lib/swap.ts:7](https://github.com/liquality/chainify/blob/540cfa69/packages/utils/lib/swap.ts#L7)

___

### validateSecret

▸ **validateSecret**(`secret`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `secret` | `string` |

#### Returns

`void`

#### Defined in

[utils/lib/swap.ts:17](https://github.com/liquality/chainify/blob/540cfa69/packages/utils/lib/swap.ts#L17)

___

### validateSecretAndHash

▸ **validateSecretAndHash**(`secret`, `secretHash`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `secret` | `string` |
| `secretHash` | `string` |

#### Returns

`void`

#### Defined in

[utils/lib/swap.ts:55](https://github.com/liquality/chainify/blob/540cfa69/packages/utils/lib/swap.ts#L55)

___

### validateSecretHash

▸ **validateSecretHash**(`secretHash`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `secretHash` | `string` |

#### Returns

`void`

#### Defined in

[utils/lib/swap.ts:34](https://github.com/liquality/chainify/blob/540cfa69/packages/utils/lib/swap.ts#L34)

___

### validateValue

▸ **validateValue**(`value`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `BigNumberish` |

#### Returns

`void`

#### Defined in

[utils/lib/swap.ts:65](https://github.com/liquality/chainify/blob/540cfa69/packages/utils/lib/swap.ts#L65)
