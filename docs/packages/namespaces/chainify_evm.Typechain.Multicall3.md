---
id: "chainify_evm.Typechain.Multicall3"
title: "Namespace: Multicall3"
sidebar_label: "Multicall3"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](chainify_evm.Typechain.md).Multicall3

## Type aliases

### Call3Struct

Ƭ **Call3Struct**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `allowFailure` | `boolean` |
| `callData` | `BytesLike` |
| `target` | `string` |

#### Defined in

evm/lib/typechain/Multicall3.ts:28

___

### Call3StructOutput

Ƭ **Call3StructOutput**: [`string`, `boolean`, `string`] & { `allowFailure`: `boolean` ; `callData`: `string` ; `target`: `string`  }

#### Defined in

evm/lib/typechain/Multicall3.ts:34

___

### Call3ValueStruct

Ƭ **Call3ValueStruct**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `allowFailure` | `boolean` |
| `callData` | `BytesLike` |
| `target` | `string` |
| `value` | `BigNumberish` |

#### Defined in

evm/lib/typechain/Multicall3.ts:47

___

### Call3ValueStructOutput

Ƭ **Call3ValueStructOutput**: [`string`, `boolean`, `BigNumber`, `string`] & { `allowFailure`: `boolean` ; `callData`: `string` ; `target`: `string` ; `value`: `BigNumber`  }

#### Defined in

evm/lib/typechain/Multicall3.ts:54

___

### CallStruct

Ƭ **CallStruct**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `callData` | `BytesLike` |
| `target` | `string` |

#### Defined in

evm/lib/typechain/Multicall3.ts:21

___

### CallStructOutput

Ƭ **CallStructOutput**: [`string`, `string`] & { `callData`: `string` ; `target`: `string`  }

#### Defined in

evm/lib/typechain/Multicall3.ts:23

___

### ResultStruct

Ƭ **ResultStruct**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `returnData` | `BytesLike` |
| `success` | `boolean` |

#### Defined in

evm/lib/typechain/Multicall3.ts:40

___

### ResultStructOutput

Ƭ **ResultStructOutput**: [`boolean`, `string`] & { `returnData`: `string` ; `success`: `boolean`  }

#### Defined in

evm/lib/typechain/Multicall3.ts:42
