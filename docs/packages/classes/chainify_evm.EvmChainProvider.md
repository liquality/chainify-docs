---
id: "chainify_evm.EvmChainProvider"
title: "Class: EvmChainProvider"
sidebar_label: "EvmChainProvider"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).EvmChainProvider

## Hierarchy

- `default`<`StaticJsonRpcProvider`\>

  ↳ **`EvmChainProvider`**

  ↳↳ [`OptimismChainProvider`](chainify_evm.OptimismChainProvider.md)

## Constructors

### constructor

• **new EvmChainProvider**(`network`, `provider?`, `feeProvider?`, `multicall?`)

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `network` | `Network` | `undefined` |  |
| `provider?` | `StaticJsonRpcProvider` | `undefined` |  |
| `feeProvider?` | `default` | `undefined` |  |
| `multicall` | `boolean` | `true` | - |

#### Overrides

Chain&lt;StaticJsonRpcProvider\&gt;.constructor

#### Defined in

[evm/lib/chain/EvmChainProvider.ts:39](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmChainProvider.ts#L39)

## Properties

### feeProvider

• `Protected` **feeProvider**: `default`

#### Inherited from

Chain.feeProvider

#### Defined in

client/dist/lib/Chain.d.ts:11

___

### multicall

• **multicall**: [`EvmMulticallProvider`](chainify_evm.EvmMulticallProvider.md)

#### Defined in

[evm/lib/chain/EvmChainProvider.ts:29](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmChainProvider.ts#L29)

___

### network

• `Protected` **network**: `Network`

#### Inherited from

Chain.network

#### Defined in

client/dist/lib/Chain.d.ts:12

___

### provider

• `Protected` **provider**: `StaticJsonRpcProvider`

#### Inherited from

Chain.provider

#### Defined in

client/dist/lib/Chain.d.ts:13

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

#### Overrides

Chain.getBalance

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

#### Overrides

Chain.getBlockByHash

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

#### Overrides

Chain.getBlockByNumber

#### Defined in

[evm/lib/chain/EvmChainProvider.ts:110](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmChainProvider.ts#L110)

___

### getBlockHeight

▸ **getBlockHeight**(): `Promise`<`number`\>

#### Returns

`Promise`<`number`\>

#### Overrides

Chain.getBlockHeight

#### Defined in

[evm/lib/chain/EvmChainProvider.ts:123](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmChainProvider.ts#L123)

___

### getFeeProvider

▸ **getFeeProvider**(): `Promise`<`default`\>

#### Returns

`Promise`<`default`\>

#### Inherited from

Chain.getFeeProvider

#### Defined in

client/dist/lib/Chain.d.ts:38

___

### getFees

▸ **getFees**(): `Promise`<`FeeDetails`\>

#### Returns

`Promise`<`FeeDetails`\>

#### Overrides

Chain.getFees

#### Defined in

[evm/lib/chain/EvmChainProvider.ts:198](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmChainProvider.ts#L198)

___

### getNetwork

▸ **getNetwork**(): `Network`

#### Returns

`Network`

#### Inherited from

Chain.getNetwork

#### Defined in

client/dist/lib/Chain.d.ts:22

___

### getProvider

▸ **getProvider**(): `StaticJsonRpcProvider`

#### Returns

`StaticJsonRpcProvider`

#### Inherited from

Chain.getProvider

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

#### Overrides

Chain.getTokenDetails

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

#### Overrides

Chain.getTransactionByHash

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

#### Overrides

Chain.sendRawTransaction

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

#### Overrides

Chain.sendRpcRequest

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

Chain.setFeeProvider

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

Chain.setNetwork

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

Chain.setProvider

#### Defined in

client/dist/lib/Chain.d.ts:30
