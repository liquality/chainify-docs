---
id: "chainify_evm.Typechain.IERC1155Receiver"
title: "Interface: IERC1155Receiver"
sidebar_label: "IERC1155Receiver"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).IERC1155Receiver

## Hierarchy

- `BaseContract`

  ↳ **`IERC1155Receiver`**

## Properties

### callStatic

• **callStatic**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `onERC1155BatchReceived` | (`operator`: `string`, `from`: `string`, `ids`: `BigNumberish`[], `values`: `BigNumberish`[], `data`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`string`\> |
| `onERC1155Received` | (`operator`: `string`, `from`: `string`, `id`: `BigNumberish`, `value`: `BigNumberish`, `data`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`string`\> |
| `supportsInterface` | (`interfaceId`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`boolean`\> |

#### Overrides

BaseContract.callStatic

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:132

___

### contractName

• **contractName**: ``"IERC1155Receiver"``

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:58

___

### estimateGas

• **estimateGas**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `onERC1155BatchReceived` | (`operator`: `string`, `from`: `string`, `ids`: `BigNumberish`[], `values`: `BigNumberish`[], `data`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |
| `onERC1155Received` | (`operator`: `string`, `from`: `string`, `id`: `BigNumberish`, `value`: `BigNumberish`, `data`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |
| `supportsInterface` | (`interfaceId`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |

#### Overrides

BaseContract.estimateGas

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:159

___

### filters

• **filters**: `Object`

#### Overrides

BaseContract.filters

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:157

___

### functions

• **functions**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `onERC1155BatchReceived` | (`operator`: `string`, `from`: `string`, `ids`: `BigNumberish`[], `values`: `BigNumberish`[], `data`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |
| `onERC1155Received` | (`operator`: `string`, `from`: `string`, `id`: `BigNumberish`, `value`: `BigNumberish`, `data`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |
| `supportsInterface` | (`interfaceId`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<[`boolean`]\> |

#### Overrides

BaseContract.functions

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:84

___

### interface

• **interface**: `IERC1155ReceiverInterface`

#### Overrides

BaseContract.interface

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:63

___

### off

• **off**: `OnEvent`<[`IERC1155Receiver`](chainify_evm.Typechain.IERC1155Receiver.md)\>

#### Overrides

BaseContract.off

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:79

___

### on

• **on**: `OnEvent`<[`IERC1155Receiver`](chainify_evm.Typechain.IERC1155Receiver.md)\>

#### Overrides

BaseContract.on

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:80

___

### once

• **once**: `OnEvent`<[`IERC1155Receiver`](chainify_evm.Typechain.IERC1155Receiver.md)\>

#### Overrides

BaseContract.once

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:81

___

### populateTransaction

• **populateTransaction**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `onERC1155BatchReceived` | (`operator`: `string`, `from`: `string`, `ids`: `BigNumberish`[], `values`: `BigNumberish`[], `data`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |
| `onERC1155Received` | (`operator`: `string`, `from`: `string`, `id`: `BigNumberish`, `value`: `BigNumberish`, `data`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |
| `supportsInterface` | (`interfaceId`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |

#### Overrides

BaseContract.populateTransaction

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:184

___

### removeListener

• **removeListener**: `OnEvent`<[`IERC1155Receiver`](chainify_evm.Typechain.IERC1155Receiver.md)\>

#### Overrides

BaseContract.removeListener

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:82

## Methods

### attach

▸ **attach**(`addressOrName`): [`IERC1155Receiver`](chainify_evm.Typechain.IERC1155Receiver.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `addressOrName` | `string` |

#### Returns

[`IERC1155Receiver`](chainify_evm.Typechain.IERC1155Receiver.md)

#### Overrides

BaseContract.attach

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:60

___

### connect

▸ **connect**(`signerOrProvider`): [`IERC1155Receiver`](chainify_evm.Typechain.IERC1155Receiver.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `signerOrProvider` | `string` \| `Provider` \| `Signer` |

#### Returns

[`IERC1155Receiver`](chainify_evm.Typechain.IERC1155Receiver.md)

#### Overrides

BaseContract.connect

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:59

___

### deployed

▸ **deployed**(): `Promise`<[`IERC1155Receiver`](chainify_evm.Typechain.IERC1155Receiver.md)\>

#### Returns

`Promise`<[`IERC1155Receiver`](chainify_evm.Typechain.IERC1155Receiver.md)\>

#### Overrides

BaseContract.deployed

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:61

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

evm/lib/typechain/IERC1155Receiver.ts:71

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

evm/lib/typechain/IERC1155Receiver.ts:74

___

### onERC1155BatchReceived

▸ **onERC1155BatchReceived**(`operator`, `from`, `ids`, `values`, `data`, `overrides?`): `Promise`<`ContractTransaction`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `operator` | `string` |
| `from` | `string` |
| `ids` | `BigNumberish`[] |
| `values` | `BigNumberish`[] |
| `data` | `BytesLike` |
| `overrides?` | `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`Promise`<`ContractTransaction`\>

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:109

___

### onERC1155Received

▸ **onERC1155Received**(`operator`, `from`, `id`, `value`, `data`, `overrides?`): `Promise`<`ContractTransaction`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `operator` | `string` |
| `from` | `string` |
| `id` | `BigNumberish` |
| `value` | `BigNumberish` |
| `data` | `BytesLike` |
| `overrides?` | `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`Promise`<`ContractTransaction`\>

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:118

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

evm/lib/typechain/IERC1155Receiver.ts:65

___

### removeAllListeners

▸ **removeAllListeners**<`TEvent`\>(`eventFilter`): [`IERC1155Receiver`](chainify_evm.Typechain.IERC1155Receiver.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `TEvent` | extends `TypedEvent`<`any`, `any`, `TEvent`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventFilter` | `TypedEventFilter`<`TEvent`\> |

#### Returns

[`IERC1155Receiver`](chainify_evm.Typechain.IERC1155Receiver.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:75

▸ **removeAllListeners**(`eventName?`): [`IERC1155Receiver`](chainify_evm.Typechain.IERC1155Receiver.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventName?` | `string` |

#### Returns

[`IERC1155Receiver`](chainify_evm.Typechain.IERC1155Receiver.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/IERC1155Receiver.ts:78

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

evm/lib/typechain/IERC1155Receiver.ts:127
