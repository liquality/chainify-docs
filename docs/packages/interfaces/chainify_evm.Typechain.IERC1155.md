---
id: "chainify_evm.Typechain.IERC1155"
title: "Interface: IERC1155"
sidebar_label: "IERC1155"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).IERC1155

## Hierarchy

- `BaseContract`

  ↳ **`IERC1155`**

## Properties

### callStatic

• **callStatic**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `balanceOf` | (`account`: `string`, `id`: `BigNumberish`, `overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `balanceOfBatch` | (`accounts`: `string`[], `ids`: `BigNumberish`[], `overrides?`: `CallOverrides`) => `Promise`<`BigNumber`[]\> |
| `isApprovedForAll` | (`account`: `string`, `operator`: `string`, `overrides?`: `CallOverrides`) => `Promise`<`boolean`\> |
| `safeBatchTransferFrom` | (`from`: `string`, `to`: `string`, `ids`: `BigNumberish`[], `amounts`: `BigNumberish`[], `data`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`void`\> |
| `safeTransferFrom` | (`from`: `string`, `to`: `string`, `id`: `BigNumberish`, `amount`: `BigNumberish`, `data`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`void`\> |
| `setApprovalForAll` | (`operator`: `string`, `approved`: `boolean`, `overrides?`: `CallOverrides`) => `Promise`<`void`\> |
| `supportsInterface` | (`interfaceId`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`boolean`\> |

#### Overrides

BaseContract.callStatic

#### Defined in

evm/lib/typechain/IERC1155.ts:263

___

### contractName

• **contractName**: ``"IERC1155"``

#### Defined in

evm/lib/typechain/IERC1155.ts:141

___

### estimateGas

• **estimateGas**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `balanceOf` | (`account`: `string`, `id`: `BigNumberish`, `overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `balanceOfBatch` | (`accounts`: `string`[], `ids`: `BigNumberish`[], `overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `isApprovedForAll` | (`account`: `string`, `operator`: `string`, `overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `safeBatchTransferFrom` | (`from`: `string`, `to`: `string`, `ids`: `BigNumberish`[], `amounts`: `BigNumberish`[], `data`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |
| `safeTransferFrom` | (`from`: `string`, `to`: `string`, `id`: `BigNumberish`, `amount`: `BigNumberish`, `data`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |
| `setApprovalForAll` | (`operator`: `string`, `approved`: `boolean`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |
| `supportsInterface` | (`interfaceId`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |

#### Overrides

BaseContract.estimateGas

#### Defined in

evm/lib/typechain/IERC1155.ts:361

___

### filters

• **filters**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `ApprovalForAll` | (`account?`: `string`, `operator?`: `string`, `approved?`: ``null``) => `ApprovalForAllEventFilter` |
| `ApprovalForAll(address,address,bool)` | (`account?`: `string`, `operator?`: `string`, `approved?`: ``null``) => `ApprovalForAllEventFilter` |
| `TransferBatch` | (`operator?`: `string`, `from?`: `string`, `to?`: `string`, `ids?`: ``null``, `values?`: ``null``) => `TransferBatchEventFilter` |
| `TransferBatch(address,address,address,uint256[],uint256[])` | (`operator?`: `string`, `from?`: `string`, `to?`: `string`, `ids?`: ``null``, `values?`: ``null``) => `TransferBatchEventFilter` |
| `TransferSingle` | (`operator?`: `string`, `from?`: `string`, `to?`: `string`, `id?`: ``null``, `value?`: ``null``) => `TransferSingleEventFilter` |
| `TransferSingle(address,address,address,uint256,uint256)` | (`operator?`: `string`, `from?`: `string`, `to?`: `string`, `id?`: ``null``, `value?`: ``null``) => `TransferSingleEventFilter` |
| `URI` | (`value?`: ``null``, `id?`: `BigNumberish`) => `URIEventFilter` |
| `URI(string,uint256)` | (`value?`: ``null``, `id?`: `BigNumberish`) => `URIEventFilter` |

#### Overrides

BaseContract.filters

#### Defined in

evm/lib/typechain/IERC1155.ts:312

___

### functions

• **functions**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `balanceOf` | (`account`: `string`, `id`: `BigNumberish`, `overrides?`: `CallOverrides`) => `Promise`<[`BigNumber`]\> |
| `balanceOfBatch` | (`accounts`: `string`[], `ids`: `BigNumberish`[], `overrides?`: `CallOverrides`) => `Promise`<[`BigNumber`[]]\> |
| `isApprovedForAll` | (`account`: `string`, `operator`: `string`, `overrides?`: `CallOverrides`) => `Promise`<[`boolean`]\> |
| `safeBatchTransferFrom` | (`from`: `string`, `to`: `string`, `ids`: `BigNumberish`[], `amounts`: `BigNumberish`[], `data`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |
| `safeTransferFrom` | (`from`: `string`, `to`: `string`, `id`: `BigNumberish`, `amount`: `BigNumberish`, `data`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |
| `setApprovalForAll` | (`operator`: `string`, `approved`: `boolean`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |
| `supportsInterface` | (`interfaceId`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<[`boolean`]\> |

#### Overrides

BaseContract.functions

#### Defined in

evm/lib/typechain/IERC1155.ts:167

___

### interface

• **interface**: `IERC1155Interface`

#### Overrides

BaseContract.interface

#### Defined in

evm/lib/typechain/IERC1155.ts:146

___

### off

• **off**: `OnEvent`<[`IERC1155`](chainify_evm.Typechain.IERC1155.md)\>

#### Overrides

BaseContract.off

#### Defined in

evm/lib/typechain/IERC1155.ts:162

___

### on

• **on**: `OnEvent`<[`IERC1155`](chainify_evm.Typechain.IERC1155.md)\>

#### Overrides

BaseContract.on

#### Defined in

evm/lib/typechain/IERC1155.ts:163

___

### once

• **once**: `OnEvent`<[`IERC1155`](chainify_evm.Typechain.IERC1155.md)\>

#### Overrides

BaseContract.once

#### Defined in

evm/lib/typechain/IERC1155.ts:164

___

### populateTransaction

• **populateTransaction**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `balanceOf` | (`account`: `string`, `id`: `BigNumberish`, `overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |
| `balanceOfBatch` | (`accounts`: `string`[], `ids`: `BigNumberish`[], `overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |
| `isApprovedForAll` | (`account`: `string`, `operator`: `string`, `overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |
| `safeBatchTransferFrom` | (`from`: `string`, `to`: `string`, `ids`: `BigNumberish`[], `amounts`: `BigNumberish`[], `data`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |
| `safeTransferFrom` | (`from`: `string`, `to`: `string`, `id`: `BigNumberish`, `amount`: `BigNumberish`, `data`: `BytesLike`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |
| `setApprovalForAll` | (`operator`: `string`, `approved`: `boolean`, `overrides?`: `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |
| `supportsInterface` | (`interfaceId`: `BytesLike`, `overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |

#### Overrides

BaseContract.populateTransaction

#### Defined in

evm/lib/typechain/IERC1155.ts:410

___

### removeListener

• **removeListener**: `OnEvent`<[`IERC1155`](chainify_evm.Typechain.IERC1155.md)\>

#### Overrides

BaseContract.removeListener

#### Defined in

evm/lib/typechain/IERC1155.ts:165

## Methods

### attach

▸ **attach**(`addressOrName`): [`IERC1155`](chainify_evm.Typechain.IERC1155.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `addressOrName` | `string` |

#### Returns

[`IERC1155`](chainify_evm.Typechain.IERC1155.md)

#### Overrides

BaseContract.attach

#### Defined in

evm/lib/typechain/IERC1155.ts:143

___

### balanceOf

▸ **balanceOf**(`account`, `id`, `overrides?`): `Promise`<`BigNumber`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `account` | `string` |
| `id` | `BigNumberish` |
| `overrides?` | `CallOverrides` |

#### Returns

`Promise`<`BigNumber`\>

#### Defined in

evm/lib/typechain/IERC1155.ts:216

___

### balanceOfBatch

▸ **balanceOfBatch**(`accounts`, `ids`, `overrides?`): `Promise`<`BigNumber`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `accounts` | `string`[] |
| `ids` | `BigNumberish`[] |
| `overrides?` | `CallOverrides` |

#### Returns

`Promise`<`BigNumber`[]\>

#### Defined in

evm/lib/typechain/IERC1155.ts:222

___

### connect

▸ **connect**(`signerOrProvider`): [`IERC1155`](chainify_evm.Typechain.IERC1155.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `signerOrProvider` | `string` \| `Provider` \| `Signer` |

#### Returns

[`IERC1155`](chainify_evm.Typechain.IERC1155.md)

#### Overrides

BaseContract.connect

#### Defined in

evm/lib/typechain/IERC1155.ts:142

___

### deployed

▸ **deployed**(): `Promise`<[`IERC1155`](chainify_evm.Typechain.IERC1155.md)\>

#### Returns

`Promise`<[`IERC1155`](chainify_evm.Typechain.IERC1155.md)\>

#### Overrides

BaseContract.deployed

#### Defined in

evm/lib/typechain/IERC1155.ts:144

___

### isApprovedForAll

▸ **isApprovedForAll**(`account`, `operator`, `overrides?`): `Promise`<`boolean`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `account` | `string` |
| `operator` | `string` |
| `overrides?` | `CallOverrides` |

#### Returns

`Promise`<`boolean`\>

#### Defined in

evm/lib/typechain/IERC1155.ts:228

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

evm/lib/typechain/IERC1155.ts:154

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

evm/lib/typechain/IERC1155.ts:157

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

evm/lib/typechain/IERC1155.ts:148

___

### removeAllListeners

▸ **removeAllListeners**<`TEvent`\>(`eventFilter`): [`IERC1155`](chainify_evm.Typechain.IERC1155.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `TEvent` | extends `TypedEvent`<`any`, `any`, `TEvent`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventFilter` | `TypedEventFilter`<`TEvent`\> |

#### Returns

[`IERC1155`](chainify_evm.Typechain.IERC1155.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/IERC1155.ts:158

▸ **removeAllListeners**(`eventName?`): [`IERC1155`](chainify_evm.Typechain.IERC1155.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventName?` | `string` |

#### Returns

[`IERC1155`](chainify_evm.Typechain.IERC1155.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/IERC1155.ts:161

___

### safeBatchTransferFrom

▸ **safeBatchTransferFrom**(`from`, `to`, `ids`, `amounts`, `data`, `overrides?`): `Promise`<`ContractTransaction`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `from` | `string` |
| `to` | `string` |
| `ids` | `BigNumberish`[] |
| `amounts` | `BigNumberish`[] |
| `data` | `BytesLike` |
| `overrides?` | `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`Promise`<`ContractTransaction`\>

#### Defined in

evm/lib/typechain/IERC1155.ts:234

___

### safeTransferFrom

▸ **safeTransferFrom**(`from`, `to`, `id`, `amount`, `data`, `overrides?`): `Promise`<`ContractTransaction`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `from` | `string` |
| `to` | `string` |
| `id` | `BigNumberish` |
| `amount` | `BigNumberish` |
| `data` | `BytesLike` |
| `overrides?` | `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`Promise`<`ContractTransaction`\>

#### Defined in

evm/lib/typechain/IERC1155.ts:243

___

### setApprovalForAll

▸ **setApprovalForAll**(`operator`, `approved`, `overrides?`): `Promise`<`ContractTransaction`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `operator` | `string` |
| `approved` | `boolean` |
| `overrides?` | `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`Promise`<`ContractTransaction`\>

#### Defined in

evm/lib/typechain/IERC1155.ts:252

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

evm/lib/typechain/IERC1155.ts:258
