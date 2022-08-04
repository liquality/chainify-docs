---
id: "chainify_logger.Logger"
title: "Class: Logger"
sidebar_label: "Logger"
custom_edit_url: null
---

[@chainify/logger](../modules/chainify_logger.md).Logger

## Constructors

### constructor

• **new Logger**(`version`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `version` | `string` |

#### Defined in

[logger/lib/index.ts:19](https://github.com/liquality/chainify/blob/540cfa69/packages/logger/lib/index.ts#L19)

## Properties

### version

• `Readonly` **version**: `string`

#### Defined in

[logger/lib/index.ts:15](https://github.com/liquality/chainify/blob/540cfa69/packages/logger/lib/index.ts#L15)

___

### levels

▪ `Static` **levels**: typeof [`LogLevel`](../enums/chainify_logger.LogLevel.md) = `LogLevel`

#### Defined in

[logger/lib/index.ts:17](https://github.com/liquality/chainify/blob/540cfa69/packages/logger/lib/index.ts#L17)

## Methods

### debug

▸ **debug**(...`args`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `...args` | `any`[] |

#### Returns

`void`

#### Defined in

[logger/lib/index.ts:23](https://github.com/liquality/chainify/blob/540cfa69/packages/logger/lib/index.ts#L23)

___

### error

▸ **error**(...`args`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `...args` | `any`[] |

#### Returns

`void`

#### Defined in

[logger/lib/index.ts:35](https://github.com/liquality/chainify/blob/540cfa69/packages/logger/lib/index.ts#L35)

___

### info

▸ **info**(...`args`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `...args` | `any`[] |

#### Returns

`void`

#### Defined in

[logger/lib/index.ts:27](https://github.com/liquality/chainify/blob/540cfa69/packages/logger/lib/index.ts#L27)

___

### warn

▸ **warn**(...`args`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `...args` | `any`[] |

#### Returns

`void`

#### Defined in

[logger/lib/index.ts:31](https://github.com/liquality/chainify/blob/540cfa69/packages/logger/lib/index.ts#L31)

___

### from

▸ `Static` **from**(`version`): [`Logger`](chainify_logger.Logger.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `version` | `string` |

#### Returns

[`Logger`](chainify_logger.Logger.md)

#### Defined in

[logger/lib/index.ts:55](https://github.com/liquality/chainify/blob/540cfa69/packages/logger/lib/index.ts#L55)

___

### globalLogger

▸ `Static` **globalLogger**(): [`Logger`](chainify_logger.Logger.md)

#### Returns

[`Logger`](chainify_logger.Logger.md)

#### Defined in

[logger/lib/index.ts:39](https://github.com/liquality/chainify/blob/540cfa69/packages/logger/lib/index.ts#L39)

___

### setLogLevel

▸ `Static` **setLogLevel**(`logLevel`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `logLevel` | [`LogLevel`](../enums/chainify_logger.LogLevel.md) |

#### Returns

`void`

#### Defined in

[logger/lib/index.ts:46](https://github.com/liquality/chainify/blob/540cfa69/packages/logger/lib/index.ts#L46)
