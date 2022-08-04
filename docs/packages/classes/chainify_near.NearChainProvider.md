---
id: "chainify_near.NearChainProvider"
title: "Class: NearChainProvider"
sidebar_label: "NearChainProvider"
custom_edit_url: null
---

[@chainify/near](../modules/chainify_near.md).NearChainProvider

## Hierarchy

- `default`<`providers.JsonRpcProvider`\>

  ↳ **`NearChainProvider`**

## Constructors

### constructor

• **new NearChainProvider**(`network`, `provider?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `network` | [`NearNetwork`](../interfaces/chainify_near.NearTypes.NearNetwork.md) |
| `provider?` | `JsonRpcProvider` |

#### Overrides

Chain&lt;providers.JsonRpcProvider\&gt;.constructor

#### Defined in

[near/lib/chain/NearChainProvider.ts:12](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/chain/NearChainProvider.ts#L12)

## Properties

### feeProvider

• `Protected` **feeProvider**: `default`

#### Inherited from

Chain.feeProvider

#### Defined in

client/dist/lib/Chain.d.ts:11

___

### network

• `Protected` **network**: `Network`

#### Inherited from

Chain.network

#### Defined in

client/dist/lib/Chain.d.ts:12

___

### provider

• `Protected` **provider**: `JsonRpcProvider`

#### Inherited from

Chain.provider

#### Defined in

client/dist/lib/Chain.d.ts:13

## Methods

### \_getBlockById

▸ **_getBlockById**(`blockId`, `includeTx`): `Promise`<`Block`<`BlockResult`, `any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `blockId` | `string` \| `number` |
| `includeTx` | `boolean` |

#### Returns

`Promise`<`Block`<`BlockResult`, `any`\>\>

#### Defined in

[near/lib/chain/NearChainProvider.ts:86](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/chain/NearChainProvider.ts#L86)

___

### getBalance

▸ **getBalance**(`addresses`, `_assets`): `Promise`<`BigNumber`[]\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `addresses` | `AddressType`[] | - |
| `_assets` | `Asset`[] |  |

#### Returns

`Promise`<`BigNumber`[]\>

#### Overrides

Chain.getBalance

#### Defined in

[near/lib/chain/NearChainProvider.ts:56](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/chain/NearChainProvider.ts#L56)

___

### getBlockByHash

▸ **getBlockByHash**(`blockHash`, `includeTx?`): `Promise`<`Block`<`BlockResult`, `Transaction`<`any`\>\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `blockHash` | `string` |
| `includeTx?` | `boolean` |

#### Returns

`Promise`<`Block`<`BlockResult`, `Transaction`<`any`\>\>\>

#### Overrides

Chain.getBlockByHash

#### Defined in

[near/lib/chain/NearChainProvider.ts:20](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/chain/NearChainProvider.ts#L20)

___

### getBlockByNumber

▸ **getBlockByNumber**(`blockNumber?`, `includeTx?`): `Promise`<`Block`<`BlockResult`, `Transaction`<`any`\>\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `blockNumber?` | `number` |
| `includeTx?` | `boolean` |

#### Returns

`Promise`<`Block`<`BlockResult`, `Transaction`<`any`\>\>\>

#### Overrides

Chain.getBlockByNumber

#### Defined in

[near/lib/chain/NearChainProvider.ts:24](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/chain/NearChainProvider.ts#L24)

___

### getBlockHeight

▸ **getBlockHeight**(): `Promise`<`number`\>

#### Returns

`Promise`<`number`\>

#### Overrides

Chain.getBlockHeight

#### Defined in

[near/lib/chain/NearChainProvider.ts:31](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/chain/NearChainProvider.ts#L31)

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

[near/lib/chain/NearChainProvider.ts:72](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/chain/NearChainProvider.ts#L72)

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

▸ **getProvider**(): `JsonRpcProvider`

#### Returns

`JsonRpcProvider`

#### Inherited from

Chain.getProvider

#### Defined in

client/dist/lib/Chain.d.ts:26

___

### getTokenDetails

▸ **getTokenDetails**(`_asset`): `Promise`<`TokenDetails`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_asset` | `string` |

#### Returns

`Promise`<`TokenDetails`\>

#### Inherited from

Chain.getTokenDetails

#### Defined in

client/dist/lib/Chain.d.ts:42

___

### getTransactionByHash

▸ **getTransactionByHash**(`txHash`): `Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txHash` | `string` |

#### Returns

`Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Overrides

Chain.getTransactionByHash

#### Defined in

[near/lib/chain/NearChainProvider.ts:36](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/chain/NearChainProvider.ts#L36)

___

### sendRawTransaction

▸ **sendRawTransaction**(`rawTransaction`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `rawTransaction` | `string` |

#### Returns

`Promise`<`string`\>

#### Overrides

Chain.sendRawTransaction

#### Defined in

[near/lib/chain/NearChainProvider.ts:78](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/chain/NearChainProvider.ts#L78)

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

[near/lib/chain/NearChainProvider.ts:82](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/chain/NearChainProvider.ts#L82)

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
| `provider` | `JsonRpcProvider` |

#### Returns

`Promise`<`void`\>

#### Inherited from

Chain.setProvider

#### Defined in

client/dist/lib/Chain.d.ts:30
