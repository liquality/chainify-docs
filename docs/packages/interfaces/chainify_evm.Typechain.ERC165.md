---
id: "chainify_evm.Typechain.ERC165"
title: "Interface: ERC165"
sidebar_label: "ERC165"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).ERC165

## Hierarchy

- `BaseContract`

  ↳ **`ERC165`**

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

evm/lib/typechain/ERC165.ts:75

___

### contractName

• **contractName**: ``"ERC165"``

#### Defined in

evm/lib/typechain/ERC165.ts:37

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

evm/lib/typechain/ERC165.ts:84

___

### filters

• **filters**: `Object`

#### Overrides

BaseContract.filters

#### Defined in

evm/lib/typechain/ERC165.ts:82

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

evm/lib/typechain/ERC165.ts:63

___

### interface

• **interface**: `ERC165Interface`

#### Overrides

BaseContract.interface

#### Defined in

evm/lib/typechain/ERC165.ts:42

___

### off

• **off**: `OnEvent`<[`ERC165`](chainify_evm.Typechain.ERC165.md)\>

#### Overrides

BaseContract.off

#### Defined in

evm/lib/typechain/ERC165.ts:58

___

### on

• **on**: `OnEvent`<[`ERC165`](chainify_evm.Typechain.ERC165.md)\>

#### Overrides

BaseContract.on

#### Defined in

evm/lib/typechain/ERC165.ts:59

___

### once

• **once**: `OnEvent`<[`ERC165`](chainify_evm.Typechain.ERC165.md)\>

#### Overrides

BaseContract.once

#### Defined in

evm/lib/typechain/ERC165.ts:60

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

evm/lib/typechain/ERC165.ts:91

___

### removeListener

• **removeListener**: `OnEvent`<[`ERC165`](chainify_evm.Typechain.ERC165.md)\>

#### Overrides

BaseContract.removeListener

#### Defined in

evm/lib/typechain/ERC165.ts:61

## Methods

### attach

▸ **attach**(`addressOrName`): [`ERC165`](chainify_evm.Typechain.ERC165.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `addressOrName` | `string` |

#### Returns

[`ERC165`](chainify_evm.Typechain.ERC165.md)

#### Overrides

BaseContract.attach

#### Defined in

evm/lib/typechain/ERC165.ts:39

___

### connect

▸ **connect**(`signerOrProvider`): [`ERC165`](chainify_evm.Typechain.ERC165.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `signerOrProvider` | `string` \| `Provider` \| `Signer` |

#### Returns

[`ERC165`](chainify_evm.Typechain.ERC165.md)

#### Overrides

BaseContract.connect

#### Defined in

evm/lib/typechain/ERC165.ts:38

___

### deployed

▸ **deployed**(): `Promise`<[`ERC165`](chainify_evm.Typechain.ERC165.md)\>

#### Returns

`Promise`<[`ERC165`](chainify_evm.Typechain.ERC165.md)\>

#### Overrides

BaseContract.deployed

#### Defined in

evm/lib/typechain/ERC165.ts:40

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

evm/lib/typechain/ERC165.ts:50

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

evm/lib/typechain/ERC165.ts:53

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

evm/lib/typechain/ERC165.ts:44

___

### removeAllListeners

▸ **removeAllListeners**<`TEvent`\>(`eventFilter`): [`ERC165`](chainify_evm.Typechain.ERC165.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `TEvent` | extends `TypedEvent`<`any`, `any`, `TEvent`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventFilter` | `TypedEventFilter`<`TEvent`\> |

#### Returns

[`ERC165`](chainify_evm.Typechain.ERC165.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/ERC165.ts:54

▸ **removeAllListeners**(`eventName?`): [`ERC165`](chainify_evm.Typechain.ERC165.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventName?` | `string` |

#### Returns

[`ERC165`](chainify_evm.Typechain.ERC165.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/ERC165.ts:57

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

evm/lib/typechain/ERC165.ts:70
