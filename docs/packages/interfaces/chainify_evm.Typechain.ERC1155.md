---
id: "chainify_evm.Typechain.ERC1155"
title: "Interface: ERC1155"
sidebar_label: "ERC1155"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).ERC1155

## Hierarchy

- `BaseContract`

  ↳ **`ERC1155`**

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
| `uri` | (`arg0`: `BigNumberish`, `overrides?`: `CallOverrides`) => `Promise`<`string`\> |

#### Overrides

BaseContract.callStatic

#### Defined in

evm/lib/typechain/ERC1155.ts:270

___

### contractName

• **contractName**: ``"ERC1155"``

#### Defined in

evm/lib/typechain/ERC1155.ts:144

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
| `uri` | (`arg0`: `BigNumberish`, `overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |

#### Overrides

BaseContract.estimateGas

#### Defined in

evm/lib/typechain/ERC1155.ts:370

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

evm/lib/typechain/ERC1155.ts:321

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
| `uri` | (`arg0`: `BigNumberish`, `overrides?`: `CallOverrides`) => `Promise`<[`string`]\> |

#### Overrides

BaseContract.functions

#### Defined in

evm/lib/typechain/ERC1155.ts:170

___

### interface

• **interface**: `ERC1155Interface`

#### Overrides

BaseContract.interface

#### Defined in

evm/lib/typechain/ERC1155.ts:149

___

### off

• **off**: `OnEvent`<[`ERC1155`](chainify_evm.Typechain.ERC1155.md)\>

#### Overrides

BaseContract.off

#### Defined in

evm/lib/typechain/ERC1155.ts:165

___

### on

• **on**: `OnEvent`<[`ERC1155`](chainify_evm.Typechain.ERC1155.md)\>

#### Overrides

BaseContract.on

#### Defined in

evm/lib/typechain/ERC1155.ts:166

___

### once

• **once**: `OnEvent`<[`ERC1155`](chainify_evm.Typechain.ERC1155.md)\>

#### Overrides

BaseContract.once

#### Defined in

evm/lib/typechain/ERC1155.ts:167

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
| `uri` | (`arg0`: `BigNumberish`, `overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |

#### Overrides

BaseContract.populateTransaction

#### Defined in

evm/lib/typechain/ERC1155.ts:421

___

### removeListener

• **removeListener**: `OnEvent`<[`ERC1155`](chainify_evm.Typechain.ERC1155.md)\>

#### Overrides

BaseContract.removeListener

#### Defined in

evm/lib/typechain/ERC1155.ts:168

## Methods

### attach

▸ **attach**(`addressOrName`): [`ERC1155`](chainify_evm.Typechain.ERC1155.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `addressOrName` | `string` |

#### Returns

[`ERC1155`](chainify_evm.Typechain.ERC1155.md)

#### Overrides

BaseContract.attach

#### Defined in

evm/lib/typechain/ERC1155.ts:146

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

evm/lib/typechain/ERC1155.ts:221

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

evm/lib/typechain/ERC1155.ts:227

___

### connect

▸ **connect**(`signerOrProvider`): [`ERC1155`](chainify_evm.Typechain.ERC1155.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `signerOrProvider` | `string` \| `Provider` \| `Signer` |

#### Returns

[`ERC1155`](chainify_evm.Typechain.ERC1155.md)

#### Overrides

BaseContract.connect

#### Defined in

evm/lib/typechain/ERC1155.ts:145

___

### deployed

▸ **deployed**(): `Promise`<[`ERC1155`](chainify_evm.Typechain.ERC1155.md)\>

#### Returns

`Promise`<[`ERC1155`](chainify_evm.Typechain.ERC1155.md)\>

#### Overrides

BaseContract.deployed

#### Defined in

evm/lib/typechain/ERC1155.ts:147

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

evm/lib/typechain/ERC1155.ts:233

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

evm/lib/typechain/ERC1155.ts:157

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

evm/lib/typechain/ERC1155.ts:160

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

evm/lib/typechain/ERC1155.ts:151

___

### removeAllListeners

▸ **removeAllListeners**<`TEvent`\>(`eventFilter`): [`ERC1155`](chainify_evm.Typechain.ERC1155.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `TEvent` | extends `TypedEvent`<`any`, `any`, `TEvent`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventFilter` | `TypedEventFilter`<`TEvent`\> |

#### Returns

[`ERC1155`](chainify_evm.Typechain.ERC1155.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/ERC1155.ts:161

▸ **removeAllListeners**(`eventName?`): [`ERC1155`](chainify_evm.Typechain.ERC1155.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventName?` | `string` |

#### Returns

[`ERC1155`](chainify_evm.Typechain.ERC1155.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/ERC1155.ts:164

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

evm/lib/typechain/ERC1155.ts:239

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

evm/lib/typechain/ERC1155.ts:248

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

evm/lib/typechain/ERC1155.ts:257

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

evm/lib/typechain/ERC1155.ts:263

___

### uri

▸ **uri**(`arg0`, `overrides?`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `arg0` | `BigNumberish` |
| `overrides?` | `CallOverrides` |

#### Returns

`Promise`<`string`\>

#### Defined in

evm/lib/typechain/ERC1155.ts:268
