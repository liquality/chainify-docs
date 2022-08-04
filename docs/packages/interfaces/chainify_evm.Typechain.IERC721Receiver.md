---
id: "chainify_evm.Typechain.IERC721Receiver"
title: "Interface: IERC721Receiver"
sidebar_label: "IERC721Receiver"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).IERC721Receiver

## Hierarchy

- `BaseContract`

  ↳ **`IERC721Receiver`**

## Properties

### callStatic

• **callStatic**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `onERC721Received` | (`operator`: `string`, `from`: `string`, `tokenId`: `BigNumberish`, `data`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`string`\> |

#### Overrides

BaseContract.callStatic

#### Defined in

evm/lib/typechain/IERC721Receiver.ts:84

___

### contractName

• **contractName**: ``"IERC721Receiver"``

#### Defined in

evm/lib/typechain/IERC721Receiver.ts:40

___

### estimateGas

• **estimateGas**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `onERC721Received` | (`operator`: `string`, `from`: `string`, `tokenId`: `BigNumberish`, `data`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |

#### Overrides

BaseContract.estimateGas

#### Defined in

evm/lib/typechain/IERC721Receiver.ts:96

___

### filters

• **filters**: `Object`

#### Overrides

BaseContract.filters

#### Defined in

evm/lib/typechain/IERC721Receiver.ts:94

___

### functions

• **functions**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `onERC721Received` | (`operator`: `string`, `from`: `string`, `tokenId`: `BigNumberish`, `data`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |

#### Overrides

BaseContract.functions

#### Defined in

evm/lib/typechain/IERC721Receiver.ts:66

___

### interface

• **interface**: `IERC721ReceiverInterface`

#### Overrides

BaseContract.interface

#### Defined in

evm/lib/typechain/IERC721Receiver.ts:45

___

### off

• **off**: `OnEvent`<[`IERC721Receiver`](chainify_evm.Typechain.IERC721Receiver.md)\>

#### Overrides

BaseContract.off

#### Defined in

evm/lib/typechain/IERC721Receiver.ts:61

___

### on

• **on**: `OnEvent`<[`IERC721Receiver`](chainify_evm.Typechain.IERC721Receiver.md)\>

#### Overrides

BaseContract.on

#### Defined in

evm/lib/typechain/IERC721Receiver.ts:62

___

### once

• **once**: `OnEvent`<[`IERC721Receiver`](chainify_evm.Typechain.IERC721Receiver.md)\>

#### Overrides

BaseContract.once

#### Defined in

evm/lib/typechain/IERC721Receiver.ts:63

___

### populateTransaction

• **populateTransaction**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `onERC721Received` | (`operator`: `string`, `from`: `string`, `tokenId`: `BigNumberish`, `data`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |

#### Overrides

BaseContract.populateTransaction

#### Defined in

evm/lib/typechain/IERC721Receiver.ts:106

___

### removeListener

• **removeListener**: `OnEvent`<[`IERC721Receiver`](chainify_evm.Typechain.IERC721Receiver.md)\>

#### Overrides

BaseContract.removeListener

#### Defined in

evm/lib/typechain/IERC721Receiver.ts:64

## Methods

### attach

▸ **attach**(`addressOrName`): [`IERC721Receiver`](chainify_evm.Typechain.IERC721Receiver.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `addressOrName` | `string` |

#### Returns

[`IERC721Receiver`](chainify_evm.Typechain.IERC721Receiver.md)

#### Overrides

BaseContract.attach

#### Defined in

evm/lib/typechain/IERC721Receiver.ts:42

___

### connect

▸ **connect**(`signerOrProvider`): [`IERC721Receiver`](chainify_evm.Typechain.IERC721Receiver.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `signerOrProvider` | `string` \| `Provider` \| `Signer` |

#### Returns

[`IERC721Receiver`](chainify_evm.Typechain.IERC721Receiver.md)

#### Overrides

BaseContract.connect

#### Defined in

evm/lib/typechain/IERC721Receiver.ts:41

___

### deployed

▸ **deployed**(): `Promise`<[`IERC721Receiver`](chainify_evm.Typechain.IERC721Receiver.md)\>

#### Returns

`Promise`<[`IERC721Receiver`](chainify_evm.Typechain.IERC721Receiver.md)\>

#### Overrides

BaseContract.deployed

#### Defined in

evm/lib/typechain/IERC721Receiver.ts:43

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

evm/lib/typechain/IERC721Receiver.ts:53

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

evm/lib/typechain/IERC721Receiver.ts:56

___

### onERC721Received

▸ **onERC721Received**(`operator`, `from`, `tokenId`, `data`, `overrides?`): `Promise`<`ContractTransaction`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `operator` | `string` |
| `from` | `string` |
| `tokenId` | `BigNumberish` |
| `data` | `BytesLike` |
| `overrides?` | `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`Promise`<`ContractTransaction`\>

#### Defined in

evm/lib/typechain/IERC721Receiver.ts:76

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

evm/lib/typechain/IERC721Receiver.ts:47

___

### removeAllListeners

▸ **removeAllListeners**<`TEvent`\>(`eventFilter`): [`IERC721Receiver`](chainify_evm.Typechain.IERC721Receiver.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `TEvent` | extends `TypedEvent`<`any`, `any`, `TEvent`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventFilter` | `TypedEventFilter`<`TEvent`\> |

#### Returns

[`IERC721Receiver`](chainify_evm.Typechain.IERC721Receiver.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/IERC721Receiver.ts:57

▸ **removeAllListeners**(`eventName?`): [`IERC721Receiver`](chainify_evm.Typechain.IERC721Receiver.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventName?` | `string` |

#### Returns

[`IERC721Receiver`](chainify_evm.Typechain.IERC721Receiver.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/IERC721Receiver.ts:60
