---
id: "chainify_evm.Typechain.LiqualityHTLC"
title: "Interface: LiqualityHTLC"
sidebar_label: "LiqualityHTLC"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).LiqualityHTLC

## Hierarchy

- `BaseContract`

  ↳ **`LiqualityHTLC`**

## Properties

### callStatic

• **callStatic**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `claim` | (`id`: `BytesLike`, `secret`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`void`\> |
| `htlcs` | (`arg0`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<[`BigNumber`, `BigNumber`, `string`, `string`, `string`, `string`] & { `amount`: `BigNumber` ; `expiration`: `BigNumber` ; `recipientAddress`: `string` ; `refundAddress`: `string` ; `secretHash`: `string` ; `tokenAddress`: `string`  }\> |
| `initiate` | (`htlc`: `HTLCDataStruct`, `overrides?`: `CallOverrides`) => `Promise`<`string`\> |
| `refund` | (`id`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`void`\> |

#### Overrides

BaseContract.callStatic

#### Defined in

evm/lib/typechain/LiqualityHTLC.ts:191

___

### contractName

• **contractName**: ``"LiqualityHTLC"``

#### Defined in

evm/lib/typechain/LiqualityHTLC.ts:103

___

### estimateGas

• **estimateGas**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `claim` | (`id`: `BytesLike`, `secret`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |
| `htlcs` | (`arg0`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `initiate` | (`htlc`: `HTLCDataStruct`, `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |
| `refund` | (`id`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |

#### Overrides

BaseContract.estimateGas

#### Defined in

evm/lib/typechain/LiqualityHTLC.ts:234

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

evm/lib/typechain/LiqualityHTLC.ts:220

___

### functions

• **functions**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `claim` | (`id`: `BytesLike`, `secret`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |
| `htlcs` | (`arg0`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<[`BigNumber`, `BigNumber`, `string`, `string`, `string`, `string`] & { `amount`: `BigNumber` ; `expiration`: `BigNumber` ; `recipientAddress`: `string` ; `refundAddress`: `string` ; `secretHash`: `string` ; `tokenAddress`: `string`  }\> |
| `initiate` | (`htlc`: `HTLCDataStruct`, `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |
| `refund` | (`id`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |

#### Overrides

BaseContract.functions

#### Defined in

evm/lib/typechain/LiqualityHTLC.ts:129

___

### interface

• **interface**: `LiqualityHTLCInterface`

#### Overrides

BaseContract.interface

#### Defined in

evm/lib/typechain/LiqualityHTLC.ts:108

___

### off

• **off**: `OnEvent`<[`LiqualityHTLC`](chainify_evm.Typechain.LiqualityHTLC.md)\>

#### Overrides

BaseContract.off

#### Defined in

evm/lib/typechain/LiqualityHTLC.ts:124

___

### on

• **on**: `OnEvent`<[`LiqualityHTLC`](chainify_evm.Typechain.LiqualityHTLC.md)\>

#### Overrides

BaseContract.on

#### Defined in

evm/lib/typechain/LiqualityHTLC.ts:125

___

### once

• **once**: `OnEvent`<[`LiqualityHTLC`](chainify_evm.Typechain.LiqualityHTLC.md)\>

#### Overrides

BaseContract.once

#### Defined in

evm/lib/typechain/LiqualityHTLC.ts:126

___

### populateTransaction

• **populateTransaction**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `claim` | (`id`: `BytesLike`, `secret`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |
| `htlcs` | (`arg0`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |
| `initiate` | (`htlc`: `HTLCDataStruct`, `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |
| `refund` | (`id`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |

#### Overrides

BaseContract.populateTransaction

#### Defined in

evm/lib/typechain/LiqualityHTLC.ts:254

___

### removeListener

• **removeListener**: `OnEvent`<[`LiqualityHTLC`](chainify_evm.Typechain.LiqualityHTLC.md)\>

#### Overrides

BaseContract.removeListener

#### Defined in

evm/lib/typechain/LiqualityHTLC.ts:127

## Methods

### attach

▸ **attach**(`addressOrName`): [`LiqualityHTLC`](chainify_evm.Typechain.LiqualityHTLC.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `addressOrName` | `string` |

#### Returns

[`LiqualityHTLC`](chainify_evm.Typechain.LiqualityHTLC.md)

#### Overrides

BaseContract.attach

#### Defined in

evm/lib/typechain/LiqualityHTLC.ts:105

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

evm/lib/typechain/LiqualityHTLC.ts:161

___

### connect

▸ **connect**(`signerOrProvider`): [`LiqualityHTLC`](chainify_evm.Typechain.LiqualityHTLC.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `signerOrProvider` | `string` \| `Provider` \| `Signer` |

#### Returns

[`LiqualityHTLC`](chainify_evm.Typechain.LiqualityHTLC.md)

#### Overrides

BaseContract.connect

#### Defined in

evm/lib/typechain/LiqualityHTLC.ts:104

___

### deployed

▸ **deployed**(): `Promise`<[`LiqualityHTLC`](chainify_evm.Typechain.LiqualityHTLC.md)\>

#### Returns

`Promise`<[`LiqualityHTLC`](chainify_evm.Typechain.LiqualityHTLC.md)\>

#### Overrides

BaseContract.deployed

#### Defined in

evm/lib/typechain/LiqualityHTLC.ts:106

___

### htlcs

▸ **htlcs**(`arg0`, `overrides?`): `Promise`<[`BigNumber`, `BigNumber`, `string`, `string`, `string`, `string`] & { `amount`: `BigNumber` ; `expiration`: `BigNumber` ; `recipientAddress`: `string` ; `refundAddress`: `string` ; `secretHash`: `string` ; `tokenAddress`: `string`  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `arg0` | `BytesLike` |
| `overrides?` | `CallOverrides` |

#### Returns

`Promise`<[`BigNumber`, `BigNumber`, `string`, `string`, `string`, `string`] & { `amount`: `BigNumber` ; `expiration`: `BigNumber` ; `recipientAddress`: `string` ; `refundAddress`: `string` ; `secretHash`: `string` ; `tokenAddress`: `string`  }\>

#### Defined in

evm/lib/typechain/LiqualityHTLC.ts:167

___

### initiate

▸ **initiate**(`htlc`, `overrides?`): `Promise`<`ContractTransaction`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `htlc` | `HTLCDataStruct` |
| `overrides?` | `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`Promise`<`ContractTransaction`\>

#### Defined in

evm/lib/typechain/LiqualityHTLC.ts:181

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

evm/lib/typechain/LiqualityHTLC.ts:116

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

evm/lib/typechain/LiqualityHTLC.ts:119

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

evm/lib/typechain/LiqualityHTLC.ts:110

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

evm/lib/typechain/LiqualityHTLC.ts:186

___

### removeAllListeners

▸ **removeAllListeners**<`TEvent`\>(`eventFilter`): [`LiqualityHTLC`](chainify_evm.Typechain.LiqualityHTLC.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `TEvent` | extends `TypedEvent`<`any`, `any`, `TEvent`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventFilter` | `TypedEventFilter`<`TEvent`\> |

#### Returns

[`LiqualityHTLC`](chainify_evm.Typechain.LiqualityHTLC.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/LiqualityHTLC.ts:120

▸ **removeAllListeners**(`eventName?`): [`LiqualityHTLC`](chainify_evm.Typechain.LiqualityHTLC.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventName?` | `string` |

#### Returns

[`LiqualityHTLC`](chainify_evm.Typechain.LiqualityHTLC.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/LiqualityHTLC.ts:123
