---
id: "chainify_evm.Typechain.ILiqualityHTLC-1"
title: "Interface: ILiqualityHTLC"
sidebar_label: "ILiqualityHTLC"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).ILiqualityHTLC

## Hierarchy

- `BaseContract`

  ↳ **`ILiqualityHTLC`**

## Properties

### callStatic

• **callStatic**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `claim` | (`id`: `BytesLike`, `secret`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`void`\> |
| `initiate` | (`htlc`: [`HTLCDataStruct`](../namespaces/chainify_evm.Typechain.ILiqualityHTLC.md#htlcdatastruct), `overrides?`: `CallOverrides`) => `Promise`<`string`\> |
| `refund` | (`id`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`void`\> |

#### Overrides

BaseContract.callStatic

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:160

___

### contractName

• **contractName**: ``"ILiqualityHTLC"``

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:100

___

### estimateGas

• **estimateGas**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `claim` | (`id`: `BytesLike`, `secret`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |
| `initiate` | (`htlc`: [`HTLCDataStruct`](../namespaces/chainify_evm.Typechain.ILiqualityHTLC.md#htlcdatastruct), `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |
| `refund` | (`id`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |

#### Overrides

BaseContract.estimateGas

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:189

___

### filters

• **filters**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `Claim` | (`id?`: `BytesLike`, `secret?`: ``null``) => `ClaimEventFilter` |
| `Claim(bytes32,bytes32)` | (`id?`: `BytesLike`, `secret?`: ``null``) => `ClaimEventFilter` |
| `Initiate` | (`id?`: ``null``, `htlc?`: ``null``) => `InitiateEventFilter` |
| `Initiate(bytes32,tuple)` | (`id?`: ``null``, `htlc?`: ``null``) => `InitiateEventFilter` |
| `Refund` | (`id?`: `BytesLike`) => `RefundEventFilter` |
| `Refund(bytes32)` | (`id?`: `BytesLike`) => `RefundEventFilter` |

#### Overrides

BaseContract.filters

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:175

___

### functions

• **functions**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `claim` | (`id`: `BytesLike`, `secret`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |
| `initiate` | (`htlc`: [`HTLCDataStruct`](../namespaces/chainify_evm.Typechain.ILiqualityHTLC.md#htlcdatastruct), `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |
| `refund` | (`id`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |

#### Overrides

BaseContract.functions

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:126

___

### interface

• **interface**: `ILiqualityHTLCInterface`

#### Overrides

BaseContract.interface

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:105

___

### off

• **off**: `OnEvent`<[`ILiqualityHTLC`](chainify_evm.Typechain.ILiqualityHTLC-1.md)\>

#### Overrides

BaseContract.off

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:121

___

### on

• **on**: `OnEvent`<[`ILiqualityHTLC`](chainify_evm.Typechain.ILiqualityHTLC-1.md)\>

#### Overrides

BaseContract.on

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:122

___

### once

• **once**: `OnEvent`<[`ILiqualityHTLC`](chainify_evm.Typechain.ILiqualityHTLC-1.md)\>

#### Overrides

BaseContract.once

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:123

___

### populateTransaction

• **populateTransaction**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `claim` | (`id`: `BytesLike`, `secret`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |
| `initiate` | (`htlc`: [`HTLCDataStruct`](../namespaces/chainify_evm.Typechain.ILiqualityHTLC.md#htlcdatastruct), `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |
| `refund` | (`id`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |

#### Overrides

BaseContract.populateTransaction

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:207

___

### removeListener

• **removeListener**: `OnEvent`<[`ILiqualityHTLC`](chainify_evm.Typechain.ILiqualityHTLC-1.md)\>

#### Overrides

BaseContract.removeListener

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:124

## Methods

### attach

▸ **attach**(`addressOrName`): [`ILiqualityHTLC`](chainify_evm.Typechain.ILiqualityHTLC-1.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `addressOrName` | `string` |

#### Returns

[`ILiqualityHTLC`](chainify_evm.Typechain.ILiqualityHTLC-1.md)

#### Overrides

BaseContract.attach

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:102

___

### claim

▸ **claim**(`id`, `secret`, `overrides?`): `Promise`<`ContractTransaction`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `BytesLike` |
| `secret` | `BytesLike` |
| `overrides?` | `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`Promise`<`ContractTransaction`\>

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:144

___

### connect

▸ **connect**(`signerOrProvider`): [`ILiqualityHTLC`](chainify_evm.Typechain.ILiqualityHTLC-1.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `signerOrProvider` | `string` \| `Provider` \| `Signer` |

#### Returns

[`ILiqualityHTLC`](chainify_evm.Typechain.ILiqualityHTLC-1.md)

#### Overrides

BaseContract.connect

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:101

___

### deployed

▸ **deployed**(): `Promise`<[`ILiqualityHTLC`](chainify_evm.Typechain.ILiqualityHTLC-1.md)\>

#### Returns

`Promise`<[`ILiqualityHTLC`](chainify_evm.Typechain.ILiqualityHTLC-1.md)\>

#### Overrides

BaseContract.deployed

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:103

___

### initiate

▸ **initiate**(`htlc`, `overrides?`): `Promise`<`ContractTransaction`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `htlc` | [`HTLCDataStruct`](../namespaces/chainify_evm.Typechain.ILiqualityHTLC.md#htlcdatastruct) |
| `overrides?` | `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`Promise`<`ContractTransaction`\>

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:150

___

### listeners

▸ **listeners**<`TEvent`\>(`eventFilter?`): `TypedListener`<`TEvent`\>[]

#### Type parameters

| Name | Type |
| :------ | :------ |
| `TEvent` | extends `TypedEvent`<`any`, `any`, `TEvent`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventFilter?` | `TypedEventFilter`<`TEvent`\> |

#### Returns

`TypedListener`<`TEvent`\>[]

#### Overrides

BaseContract.listeners

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:113

▸ **listeners**(`eventName?`): `Listener`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventName?` | `string` |

#### Returns

`Listener`[]

#### Overrides

BaseContract.listeners

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:116

___

### queryFilter

▸ **queryFilter**<`TEvent`\>(`event`, `fromBlockOrBlockhash?`, `toBlock?`): `Promise`<`TEvent`[]\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `TEvent` | extends `TypedEvent`<`any`, `any`, `TEvent`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `event` | `TypedEventFilter`<`TEvent`\> |
| `fromBlockOrBlockhash?` | `string` \| `number` |
| `toBlock?` | `string` \| `number` |

#### Returns

`Promise`<`TEvent`[]\>

#### Overrides

BaseContract.queryFilter

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:107

___

### refund

▸ **refund**(`id`, `overrides?`): `Promise`<`ContractTransaction`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `BytesLike` |
| `overrides?` | `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`Promise`<`ContractTransaction`\>

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:155

___

### removeAllListeners

▸ **removeAllListeners**<`TEvent`\>(`eventFilter`): [`ILiqualityHTLC`](chainify_evm.Typechain.ILiqualityHTLC-1.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `TEvent` | extends `TypedEvent`<`any`, `any`, `TEvent`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventFilter` | `TypedEventFilter`<`TEvent`\> |

#### Returns

[`ILiqualityHTLC`](chainify_evm.Typechain.ILiqualityHTLC-1.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:117

▸ **removeAllListeners**(`eventName?`): [`ILiqualityHTLC`](chainify_evm.Typechain.ILiqualityHTLC-1.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventName?` | `string` |

#### Returns

[`ILiqualityHTLC`](chainify_evm.Typechain.ILiqualityHTLC-1.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:120
