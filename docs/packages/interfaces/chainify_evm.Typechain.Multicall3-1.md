---
id: "chainify_evm.Typechain.Multicall3-1"
title: "Interface: Multicall3"
sidebar_label: "Multicall3"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).Multicall3

## Hierarchy

- `BaseContract`

  ↳ **`Multicall3`**

## Properties

### callStatic

• **callStatic**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `aggregate` | (`calls`: [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[], `overrides?`: `CallOverrides`) => `Promise`<[`BigNumber`, `string`[]] & { `blockNumber`: `BigNumber` ; `returnData`: `string`[]  }\> |
| `aggregate3` | (`calls`: [`Call3Struct`](../namespaces/chainify_evm.Typechain.Multicall3.md#call3struct)[], `overrides?`: `CallOverrides`) => `Promise`<[`ResultStructOutput`](../namespaces/chainify_evm.Typechain.Multicall3.md#resultstructoutput)[]\> |
| `aggregate3Value` | (`calls`: [`Call3ValueStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#call3valuestruct)[], `overrides?`: `CallOverrides`) => `Promise`<[`ResultStructOutput`](../namespaces/chainify_evm.Typechain.Multicall3.md#resultstructoutput)[]\> |
| `blockAndAggregate` | (`calls`: [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[], `overrides?`: `CallOverrides`) => `Promise`<[`BigNumber`, `string`, [`ResultStructOutput`](../namespaces/chainify_evm.Typechain.Multicall3.md#resultstructoutput)[]] & { `blockHash`: `string` ; `blockNumber`: `BigNumber` ; `returnData`: [`ResultStructOutput`](../namespaces/chainify_evm.Typechain.Multicall3.md#resultstructoutput)[]  }\> |
| `getBasefee` | (`overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `getBlockHash` | (`blockNumber`: `BigNumberish`, `overrides?`: `CallOverrides`) => `Promise`<`string`\> |
| `getBlockNumber` | (`overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `getChainId` | (`overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `getCurrentBlockCoinbase` | (`overrides?`: `CallOverrides`) => `Promise`<`string`\> |
| `getCurrentBlockDifficulty` | (`overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `getCurrentBlockGasLimit` | (`overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `getCurrentBlockTimestamp` | (`overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `getEthBalance` | (`addr`: `string`, `overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `getLastBlockHash` | (`overrides?`: `CallOverrides`) => `Promise`<`string`\> |
| `tryAggregate` | (`requireSuccess`: `boolean`, `calls`: [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[], `overrides?`: `CallOverrides`) => `Promise`<[`ResultStructOutput`](../namespaces/chainify_evm.Typechain.Multicall3.md#resultstructoutput)[]\> |
| `tryBlockAndAggregate` | (`requireSuccess`: `boolean`, `calls`: [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[], `overrides?`: `CallOverrides`) => `Promise`<[`BigNumber`, `string`, [`ResultStructOutput`](../namespaces/chainify_evm.Typechain.Multicall3.md#resultstructoutput)[]] & { `blockHash`: `string` ; `blockNumber`: `BigNumber` ; `returnData`: [`ResultStructOutput`](../namespaces/chainify_evm.Typechain.Multicall3.md#resultstructoutput)[]  }\> |

#### Overrides

BaseContract.callStatic

#### Defined in

evm/lib/typechain/Multicall3.ts:362

___

### contractName

• **contractName**: ``"Multicall3"``

#### Defined in

evm/lib/typechain/Multicall3.ts:205

___

### estimateGas

• **estimateGas**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `aggregate` | (`calls`: [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |
| `aggregate3` | (`calls`: [`Call3Struct`](../namespaces/chainify_evm.Typechain.Multicall3.md#call3struct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |
| `aggregate3Value` | (`calls`: [`Call3ValueStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#call3valuestruct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |
| `blockAndAggregate` | (`calls`: [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |
| `getBasefee` | (`overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `getBlockHash` | (`blockNumber`: `BigNumberish`, `overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `getBlockNumber` | (`overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `getChainId` | (`overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `getCurrentBlockCoinbase` | (`overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `getCurrentBlockDifficulty` | (`overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `getCurrentBlockGasLimit` | (`overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `getCurrentBlockTimestamp` | (`overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `getEthBalance` | (`addr`: `string`, `overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `getLastBlockHash` | (`overrides?`: `CallOverrides`) => `Promise`<`BigNumber`\> |
| `tryAggregate` | (`requireSuccess`: `boolean`, `calls`: [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |
| `tryBlockAndAggregate` | (`requireSuccess`: `boolean`, `calls`: [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`BigNumber`\> |

#### Overrides

BaseContract.estimateGas

#### Defined in

evm/lib/typechain/Multicall3.ts:435

___

### filters

• **filters**: `Object`

#### Overrides

BaseContract.filters

#### Defined in

evm/lib/typechain/Multicall3.ts:433

___

### functions

• **functions**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `aggregate` | (`calls`: [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |
| `aggregate3` | (`calls`: [`Call3Struct`](../namespaces/chainify_evm.Typechain.Multicall3.md#call3struct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |
| `aggregate3Value` | (`calls`: [`Call3ValueStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#call3valuestruct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |
| `blockAndAggregate` | (`calls`: [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |
| `getBasefee` | (`overrides?`: `CallOverrides`) => `Promise`<[`BigNumber`] & { `basefee`: `BigNumber`  }\> |
| `getBlockHash` | (`blockNumber`: `BigNumberish`, `overrides?`: `CallOverrides`) => `Promise`<[`string`] & { `blockHash`: `string`  }\> |
| `getBlockNumber` | (`overrides?`: `CallOverrides`) => `Promise`<[`BigNumber`] & { `blockNumber`: `BigNumber`  }\> |
| `getChainId` | (`overrides?`: `CallOverrides`) => `Promise`<[`BigNumber`] & { `chainid`: `BigNumber`  }\> |
| `getCurrentBlockCoinbase` | (`overrides?`: `CallOverrides`) => `Promise`<[`string`] & { `coinbase`: `string`  }\> |
| `getCurrentBlockDifficulty` | (`overrides?`: `CallOverrides`) => `Promise`<[`BigNumber`] & { `difficulty`: `BigNumber`  }\> |
| `getCurrentBlockGasLimit` | (`overrides?`: `CallOverrides`) => `Promise`<[`BigNumber`] & { `gaslimit`: `BigNumber`  }\> |
| `getCurrentBlockTimestamp` | (`overrides?`: `CallOverrides`) => `Promise`<[`BigNumber`] & { `timestamp`: `BigNumber`  }\> |
| `getEthBalance` | (`addr`: `string`, `overrides?`: `CallOverrides`) => `Promise`<[`BigNumber`] & { `balance`: `BigNumber`  }\> |
| `getLastBlockHash` | (`overrides?`: `CallOverrides`) => `Promise`<[`string`] & { `blockHash`: `string`  }\> |
| `tryAggregate` | (`requireSuccess`: `boolean`, `calls`: [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |
| `tryBlockAndAggregate` | (`requireSuccess`: `boolean`, `calls`: [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`ContractTransaction`\> |

#### Overrides

BaseContract.functions

#### Defined in

evm/lib/typechain/Multicall3.ts:231

___

### interface

• **interface**: `Multicall3Interface`

#### Overrides

BaseContract.interface

#### Defined in

evm/lib/typechain/Multicall3.ts:210

___

### off

• **off**: `OnEvent`<[`Multicall3`](chainify_evm.Typechain.Multicall3-1.md)\>

#### Overrides

BaseContract.off

#### Defined in

evm/lib/typechain/Multicall3.ts:226

___

### on

• **on**: `OnEvent`<[`Multicall3`](chainify_evm.Typechain.Multicall3-1.md)\>

#### Overrides

BaseContract.on

#### Defined in

evm/lib/typechain/Multicall3.ts:227

___

### once

• **once**: `OnEvent`<[`Multicall3`](chainify_evm.Typechain.Multicall3-1.md)\>

#### Overrides

BaseContract.once

#### Defined in

evm/lib/typechain/Multicall3.ts:228

___

### populateTransaction

• **populateTransaction**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `aggregate` | (`calls`: [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |
| `aggregate3` | (`calls`: [`Call3Struct`](../namespaces/chainify_evm.Typechain.Multicall3.md#call3struct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |
| `aggregate3Value` | (`calls`: [`Call3ValueStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#call3valuestruct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |
| `blockAndAggregate` | (`calls`: [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |
| `getBasefee` | (`overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |
| `getBlockHash` | (`blockNumber`: `BigNumberish`, `overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |
| `getBlockNumber` | (`overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |
| `getChainId` | (`overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |
| `getCurrentBlockCoinbase` | (`overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |
| `getCurrentBlockDifficulty` | (`overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |
| `getCurrentBlockGasLimit` | (`overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |
| `getCurrentBlockTimestamp` | (`overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |
| `getEthBalance` | (`addr`: `string`, `overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |
| `getLastBlockHash` | (`overrides?`: `CallOverrides`) => `Promise`<`PopulatedTransaction`\> |
| `tryAggregate` | (`requireSuccess`: `boolean`, `calls`: [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |
| `tryBlockAndAggregate` | (`requireSuccess`: `boolean`, `calls`: [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[], `overrides?`: `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  }) => `Promise`<`PopulatedTransaction`\> |

#### Overrides

BaseContract.populateTransaction

#### Defined in

evm/lib/typechain/Multicall3.ts:492

___

### removeListener

• **removeListener**: `OnEvent`<[`Multicall3`](chainify_evm.Typechain.Multicall3-1.md)\>

#### Overrides

BaseContract.removeListener

#### Defined in

evm/lib/typechain/Multicall3.ts:229

## Methods

### aggregate

▸ **aggregate**(`calls`, `overrides?`): `Promise`<`ContractTransaction`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `calls` | [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[] |
| `overrides?` | `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`Promise`<`ContractTransaction`\>

#### Defined in

evm/lib/typechain/Multicall3.ts:307

___

### aggregate3

▸ **aggregate3**(`calls`, `overrides?`): `Promise`<`ContractTransaction`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `calls` | [`Call3Struct`](../namespaces/chainify_evm.Typechain.Multicall3.md#call3struct)[] |
| `overrides?` | `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`Promise`<`ContractTransaction`\>

#### Defined in

evm/lib/typechain/Multicall3.ts:312

___

### aggregate3Value

▸ **aggregate3Value**(`calls`, `overrides?`): `Promise`<`ContractTransaction`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `calls` | [`Call3ValueStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#call3valuestruct)[] |
| `overrides?` | `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`Promise`<`ContractTransaction`\>

#### Defined in

evm/lib/typechain/Multicall3.ts:317

___

### attach

▸ **attach**(`addressOrName`): [`Multicall3`](chainify_evm.Typechain.Multicall3-1.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `addressOrName` | `string` |

#### Returns

[`Multicall3`](chainify_evm.Typechain.Multicall3-1.md)

#### Overrides

BaseContract.attach

#### Defined in

evm/lib/typechain/Multicall3.ts:207

___

### blockAndAggregate

▸ **blockAndAggregate**(`calls`, `overrides?`): `Promise`<`ContractTransaction`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `calls` | [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[] |
| `overrides?` | `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`Promise`<`ContractTransaction`\>

#### Defined in

evm/lib/typechain/Multicall3.ts:322

___

### connect

▸ **connect**(`signerOrProvider`): [`Multicall3`](chainify_evm.Typechain.Multicall3-1.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `signerOrProvider` | `string` \| `Provider` \| `Signer` |

#### Returns

[`Multicall3`](chainify_evm.Typechain.Multicall3-1.md)

#### Overrides

BaseContract.connect

#### Defined in

evm/lib/typechain/Multicall3.ts:206

___

### deployed

▸ **deployed**(): `Promise`<[`Multicall3`](chainify_evm.Typechain.Multicall3-1.md)\>

#### Returns

`Promise`<[`Multicall3`](chainify_evm.Typechain.Multicall3-1.md)\>

#### Overrides

BaseContract.deployed

#### Defined in

evm/lib/typechain/Multicall3.ts:208

___

### getBasefee

▸ **getBasefee**(`overrides?`): `Promise`<`BigNumber`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `overrides?` | `CallOverrides` |

#### Returns

`Promise`<`BigNumber`\>

#### Defined in

evm/lib/typechain/Multicall3.ts:327

___

### getBlockHash

▸ **getBlockHash**(`blockNumber`, `overrides?`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `blockNumber` | `BigNumberish` |
| `overrides?` | `CallOverrides` |

#### Returns

`Promise`<`string`\>

#### Defined in

evm/lib/typechain/Multicall3.ts:329

___

### getBlockNumber

▸ **getBlockNumber**(`overrides?`): `Promise`<`BigNumber`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `overrides?` | `CallOverrides` |

#### Returns

`Promise`<`BigNumber`\>

#### Defined in

evm/lib/typechain/Multicall3.ts:334

___

### getChainId

▸ **getChainId**(`overrides?`): `Promise`<`BigNumber`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `overrides?` | `CallOverrides` |

#### Returns

`Promise`<`BigNumber`\>

#### Defined in

evm/lib/typechain/Multicall3.ts:336

___

### getCurrentBlockCoinbase

▸ **getCurrentBlockCoinbase**(`overrides?`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `overrides?` | `CallOverrides` |

#### Returns

`Promise`<`string`\>

#### Defined in

evm/lib/typechain/Multicall3.ts:338

___

### getCurrentBlockDifficulty

▸ **getCurrentBlockDifficulty**(`overrides?`): `Promise`<`BigNumber`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `overrides?` | `CallOverrides` |

#### Returns

`Promise`<`BigNumber`\>

#### Defined in

evm/lib/typechain/Multicall3.ts:340

___

### getCurrentBlockGasLimit

▸ **getCurrentBlockGasLimit**(`overrides?`): `Promise`<`BigNumber`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `overrides?` | `CallOverrides` |

#### Returns

`Promise`<`BigNumber`\>

#### Defined in

evm/lib/typechain/Multicall3.ts:342

___

### getCurrentBlockTimestamp

▸ **getCurrentBlockTimestamp**(`overrides?`): `Promise`<`BigNumber`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `overrides?` | `CallOverrides` |

#### Returns

`Promise`<`BigNumber`\>

#### Defined in

evm/lib/typechain/Multicall3.ts:344

___

### getEthBalance

▸ **getEthBalance**(`addr`, `overrides?`): `Promise`<`BigNumber`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `addr` | `string` |
| `overrides?` | `CallOverrides` |

#### Returns

`Promise`<`BigNumber`\>

#### Defined in

evm/lib/typechain/Multicall3.ts:346

___

### getLastBlockHash

▸ **getLastBlockHash**(`overrides?`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `overrides?` | `CallOverrides` |

#### Returns

`Promise`<`string`\>

#### Defined in

evm/lib/typechain/Multicall3.ts:348

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

evm/lib/typechain/Multicall3.ts:218

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

evm/lib/typechain/Multicall3.ts:221

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

evm/lib/typechain/Multicall3.ts:212

___

### removeAllListeners

▸ **removeAllListeners**<`TEvent`\>(`eventFilter`): [`Multicall3`](chainify_evm.Typechain.Multicall3-1.md)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `TEvent` | extends `TypedEvent`<`any`, `any`, `TEvent`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventFilter` | `TypedEventFilter`<`TEvent`\> |

#### Returns

[`Multicall3`](chainify_evm.Typechain.Multicall3-1.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/Multicall3.ts:222

▸ **removeAllListeners**(`eventName?`): [`Multicall3`](chainify_evm.Typechain.Multicall3-1.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `eventName?` | `string` |

#### Returns

[`Multicall3`](chainify_evm.Typechain.Multicall3-1.md)

#### Overrides

BaseContract.removeAllListeners

#### Defined in

evm/lib/typechain/Multicall3.ts:225

___

### tryAggregate

▸ **tryAggregate**(`requireSuccess`, `calls`, `overrides?`): `Promise`<`ContractTransaction`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `requireSuccess` | `boolean` |
| `calls` | [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[] |
| `overrides?` | `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`Promise`<`ContractTransaction`\>

#### Defined in

evm/lib/typechain/Multicall3.ts:350

___

### tryBlockAndAggregate

▸ **tryBlockAndAggregate**(`requireSuccess`, `calls`, `overrides?`): `Promise`<`ContractTransaction`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `requireSuccess` | `boolean` |
| `calls` | [`CallStruct`](../namespaces/chainify_evm.Typechain.Multicall3.md#callstruct)[] |
| `overrides?` | `PayableOverrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`Promise`<`ContractTransaction`\>

#### Defined in

evm/lib/typechain/Multicall3.ts:356
