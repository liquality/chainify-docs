---
id: "chainify_evm.OptimismChainProvider"
title: "Class: OptimismChainProvider"
sidebar_label: "OptimismChainProvider"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).OptimismChainProvider

## Hierarchy

- [`EvmChainProvider`](chainify_evm.EvmChainProvider.md)

  ↳ **`OptimismChainProvider`**

## Constructors

### constructor

• **new OptimismChainProvider**(`network`, `provider`, `feeOptions?`, `multicall?`)

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `network` | `Network` | `undefined` |
| `provider` | `L2Provider`<`StaticJsonRpcProvider`\> | `undefined` |
| `feeOptions?` | [`FeeOptions`](../namespaces/chainify_evm.EvmTypes.md#feeoptions) | `undefined` |
| `multicall` | `boolean` | `true` |

#### Overrides

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[constructor](chainify_evm.EvmChainProvider.md#constructor)

#### Defined in

[evm/lib/chain/OptimismChainProvider.ts:12](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/OptimismChainProvider.ts#L12)

## Properties

### feeProvider

• `Protected` **feeProvider**: `default`

#### Inherited from

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[feeProvider](chainify_evm.EvmChainProvider.md#feeprovider)

#### Defined in

client/dist/lib/Chain.d.ts:11

___

### multicall

• **multicall**: [`EvmMulticallProvider`](chainify_evm.EvmMulticallProvider.md)

#### Inherited from

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[multicall](chainify_evm.EvmChainProvider.md#multicall)

#### Defined in

[evm/lib/chain/EvmChainProvider.ts:29](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmChainProvider.ts#L29)

___

### network

• `Protected` **network**: `Network`

#### Inherited from

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[network](chainify_evm.EvmChainProvider.md#network)

#### Defined in

client/dist/lib/Chain.d.ts:12

___

### provider

• `Protected` **provider**: `L2Provider`<`StaticJsonRpcProvider`\>

#### Overrides

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[provider](chainify_evm.EvmChainProvider.md#provider)

#### Defined in

[evm/lib/chain/OptimismChainProvider.ts:10](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/OptimismChainProvider.ts#L10)

## Methods

### getBalance

▸ **getBalance**(`addresses`, `assets`): `Promise`<`BigNumber`[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `addresses` | `AddressType`[] |  |
| `assets` | `Asset`[] |  |

#### Returns

`Promise`<`BigNumber`[]\>

#### Inherited from

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[getBalance](chainify_evm.EvmChainProvider.md#getbalance)

#### Defined in

[evm/lib/chain/EvmChainProvider.ts:154](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmChainProvider.ts#L154)

___

### getBlockByHash

▸ **getBlockByHash**(`blockHash`, `includeTx?`): `Promise`<`Block`<`Block` \| `BlockWithTransactions`, `TransactionResponse`\>\>

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `blockHash` | `string` | `undefined` |  |
| `includeTx` | `boolean` | `false` | - |

#### Returns

`Promise`<`Block`<`Block` \| `BlockWithTransactions`, `TransactionResponse`\>\>

#### Inherited from

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[getBlockByHash](chainify_evm.EvmChainProvider.md#getblockbyhash)

#### Defined in

[evm/lib/chain/EvmChainProvider.ts:95](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmChainProvider.ts#L95)

___

### getBlockByNumber

▸ **getBlockByNumber**(`blockNumber?`, `includeTx?`): `Promise`<`Block`<`Block` \| `BlockWithTransactions`, `TransactionResponse`\>\>

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `blockNumber?` | `number` | `undefined` |  |
| `includeTx` | `boolean` | `false` | - |

#### Returns

`Promise`<`Block`<`Block` \| `BlockWithTransactions`, `TransactionResponse`\>\>

#### Inherited from

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[getBlockByNumber](chainify_evm.EvmChainProvider.md#getblockbynumber)

#### Defined in

[evm/lib/chain/EvmChainProvider.ts:110](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmChainProvider.ts#L110)

___

### getBlockHeight

▸ **getBlockHeight**(): `Promise`<`number`\>

#### Returns

`Promise`<`number`\>

#### Inherited from

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[getBlockHeight](chainify_evm.EvmChainProvider.md#getblockheight)

#### Defined in

[evm/lib/chain/EvmChainProvider.ts:123](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmChainProvider.ts#L123)

___

### getFeeProvider

▸ **getFeeProvider**(): `Promise`<`default`\>

#### Returns

`Promise`<`default`\>

#### Inherited from

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[getFeeProvider](chainify_evm.EvmChainProvider.md#getfeeprovider)

#### Defined in

client/dist/lib/Chain.d.ts:38

___

### getFees

▸ **getFees**(): `Promise`<`FeeDetails`\>

#### Returns

`Promise`<`FeeDetails`\>

#### Overrides

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[getFees](chainify_evm.EvmChainProvider.md#getfees)

#### Defined in

[evm/lib/chain/OptimismChainProvider.ts:22](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/OptimismChainProvider.ts#L22)

___

### getNetwork

▸ **getNetwork**(): `Network`

#### Returns

`Network`

#### Inherited from

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[getNetwork](chainify_evm.EvmChainProvider.md#getnetwork)

#### Defined in

client/dist/lib/Chain.d.ts:22

___

### getProvider

▸ **getProvider**(): `StaticJsonRpcProvider`

#### Returns

`StaticJsonRpcProvider`

#### Inherited from

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[getProvider](chainify_evm.EvmChainProvider.md#getprovider)

#### Defined in

client/dist/lib/Chain.d.ts:26

___

### getTokenDetails

▸ **getTokenDetails**(`asset`): `Promise`<`TokenDetails`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `asset` | `string` |  |

#### Returns

`Promise`<`TokenDetails`\>

#### Inherited from

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[getTokenDetails](chainify_evm.EvmChainProvider.md#gettokendetails)

#### Defined in

[evm/lib/chain/EvmChainProvider.ts:62](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmChainProvider.ts#L62)

___

### getTransactionByHash

▸ **getTransactionByHash**(`txHash`): `Promise`<`Transaction`<`TransactionResponse`\>\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `txHash` | `string` |  |

#### Returns

`Promise`<`Transaction`<`TransactionResponse`\>\>

#### Inherited from

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[getTransactionByHash](chainify_evm.EvmChainProvider.md#gettransactionbyhash)

#### Defined in

[evm/lib/chain/EvmChainProvider.ts:132](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmChainProvider.ts#L132)

___

### sendRawTransaction

▸ **sendRawTransaction**(`rawTransaction`): `Promise`<`string`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rawTransaction` | `string` |  |

#### Returns

`Promise`<`string`\>

#### Inherited from

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[sendRawTransaction](chainify_evm.EvmChainProvider.md#sendrawtransaction)

#### Defined in

[evm/lib/chain/EvmChainProvider.ts:190](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmChainProvider.ts#L190)

___

### sendRpcRequest

▸ **sendRpcRequest**(`method`, `params`): `Promise`<`any`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `method` | `string` |
| `params` | `any`[] |

#### Returns

`Promise`<`any`\>

#### Inherited from

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[sendRpcRequest](chainify_evm.EvmChainProvider.md#sendrpcrequest)

#### Defined in

[evm/lib/chain/EvmChainProvider.ts:205](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmChainProvider.ts#L205)

___

### setFeeProvider

▸ **setFeeProvider**(`feeProvider`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `feeProvider` | `default` |

#### Returns

`Promise`<`void`\>

#### Inherited from

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[setFeeProvider](chainify_evm.EvmChainProvider.md#setfeeprovider)

#### Defined in

client/dist/lib/Chain.d.ts:34

___

### setNetwork

▸ **setNetwork**(`network`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `network` | `Network` |

#### Returns

`void`

#### Inherited from

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[setNetwork](chainify_evm.EvmChainProvider.md#setnetwork)

#### Defined in

client/dist/lib/Chain.d.ts:18

___

### setProvider

▸ **setProvider**(`provider`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `provider` | `StaticJsonRpcProvider` |

#### Returns

`Promise`<`void`\>

#### Inherited from

[EvmChainProvider](chainify_evm.EvmChainProvider.md).[setProvider](chainify_evm.EvmChainProvider.md#setprovider)

#### Defined in

client/dist/lib/Chain.d.ts:30
