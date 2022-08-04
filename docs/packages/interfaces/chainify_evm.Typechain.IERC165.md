---
id: "chainify_evm.Typechain.IERC165"
title: "Interface: IERC165"
sidebar_label: "IERC165"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).IERC165

## Hierarchy

- `BaseContract`

  ↳ **`IERC165`**

## Properties

### callStatic

• **callStatic**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `supportsInterface` | (`interfaceId`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`boolean`\> |

#### Overrides

BaseContract.callStatic

#### Defined in

evm/lib/typechain/IERC165.ts:75

___

### contractName

• **contractName**: ``"IERC165"``

#### Defined in

evm/lib/typechain/IERC165.ts:37

___

### estimateGas

• **estimateGas**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `supportsInterface` | (`interfaceId`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |

#### Overrides

BaseContract.estimateGas

#### Defined in

evm/lib/typechain/IERC165.ts:84

___

### filters

• **filters**: `Object`

#### Overrides

BaseContract.filters

#### Defined in

evm/lib/typechain/IERC165.ts:82

___

### functions

• **functions**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `supportsInterface` | (`interfaceId`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<[`boolean`]\> |

#### Overrides

BaseContract.functions

#### Defined in

evm/lib/typechain/IERC165.ts:63

___

### interface

• **interface**: `IERC165Interface`

#### Overrides

BaseContract.interface

#### Defined in

evm/lib/typechain/IERC165.ts:42

___

### off

• **off**: `OnEvent`<[`IERC165`](chainify_evm.Typechain.IERC165.md)\>

#### Overrides

BaseContract.off

#### Defined in

evm/lib/typechain/IERC165.ts:58

___

### on

• **on**: `OnEvent`<[`IERC165`](chainify_evm.Typechain.IERC165.md)\>

#### Overrides

BaseContract.on

#### Defined in

evm/lib/typechain/IERC165.ts:59

___

### once

• **once**: `OnEvent`<[`IERC165`](chainify_evm.Typechain.IERC165.md)\>

#### Overrides

BaseContract.once

#### Defined in

evm/lib/typechain/IERC165.ts:60

___

### populateTransaction

• **populateTransaction**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `supportsInterface` | (`interfaceId`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |

#### Overrides

BaseContract.populateTransaction

#### Defined in

evm/lib/typechain/IERC165.ts:91

___

### removeListener

• **removeListener**: `OnEvent`<[`IERC165`](chainify_evm.Typechain.IERC165.md)\>

#### Overrides

BaseContract.removeListener

#### Defined in

evm/lib/typechain/IERC165.ts:61

## Methods

### attach

▸ **attach**(`addressOrName`): [`IERC165`](chainify_evm.Typechain.IERC165.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `addressOrName` | `string` |

#### Returns

[`IERC165`](chainify_evm.Typechain.IERC165.md)

#### Overrides

BaseContract.attach

#### Defined in

evm/lib/typechain/IERC165.ts:39

___

### connect

▸ **connect**(`signerOrProvider`): [`IERC165`](chainify_evm.Typechain.IERC165.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `signerOrProvider` | `string` \| `Provider` \| `Signer` |

#### Returns

[`IERC165`](chainify_evm.Typechain.IERC165.md)

#### Overrides

BaseContract.connect

#### Defined in

evm/lib/typechain/IERC165.ts:38

___

### deployed

▸ **deployed**(): `Promise`<[`IERC165`](chainify_evm.Typechain.IERC165.md)\>

#### Returns

`Promise`<[`IERC165`](chainify_evm.Typechain.IERC165.md)\>

#### Overrides

BaseContract.deployed

#### Defined in

evm/lib/typechain/IERC165.ts:40

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

evm/lib/typechain/IERC165.ts:50

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

evm/lib/typechain/IERC165.ts:53

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

evm/lib/typechain/IERC165.ts:44

___

### removeAllListeners

▸ **removeAllListeners**<`TEvent`\>(`eventFilter`): [`IERC165`](chainify_evm.Typechain.IERC165.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `TEvent` | extends `TypedEvent`<`any`, `any`, `TEvent`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventFilter` | `TypedEventFilter`<`TEvent`\> |

#### Returns

[`IERC165`](chainify_evm.Typechain.IERC165.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/IERC165.ts:54

▸ **removeAllListeners**(`eventName?`): [`IERC165`](chainify_evm.Typechain.IERC165.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventName?` | `string` |

#### Returns

[`IERC165`](chainify_evm.Typechain.IERC165.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/IERC165.ts:57

___

### supportsInterface

▸ **supportsInterface**(`interfaceId`, `overrides?`): `Promise`<`boolean`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `interfaceId` | `BytesLike` |
| `overrides?` | `CallOverrides` |

#### Returns

`Promise`<`boolean`\>

#### Defined in

evm/lib/typechain/IERC165.ts:70
