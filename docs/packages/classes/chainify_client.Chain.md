---
id: "chainify_client.Chain"
title: "Class: Chain<T, N>"
sidebar_label: "Chain"
custom_edit_url: null
---

[@chainify/client](../modules/chainify_client.md).Chain

## Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `T` | `T` | - |
| `N` | extends `Network` = `Network` | - |

## Implements

- `ChainProvider`

## Constructors

### constructor

• **new Chain**<`T`, `N`\>(`network`, `provider?`, `feeProvider?`)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `T` |
| `N` | extends `Network` = `Network` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `network` | `N` |
| `provider?` | `T` |
| `feeProvider?` | [`Fee`](chainify_client.Fee.md) |

#### Defined in

[client/lib/Chain.ts:28](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L28)

## Properties

### feeProvider

• `Protected` **feeProvider**: [`Fee`](chainify_client.Fee.md)

#### Defined in

[client/lib/Chain.ts:24](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L24)

___

### network

• `Protected` **network**: `N`

#### Defined in

[client/lib/Chain.ts:25](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L25)

___

### provider

• `Protected` **provider**: `T`

#### Defined in

[client/lib/Chain.ts:26](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L26)

## Methods

### getBalance

▸ `Abstract` **getBalance**(`addresses`, `assets`): `Promise`<`BigNumber`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `addresses` | `AddressType`[] |
| `assets` | `Asset`[] |

#### Returns

`Promise`<`BigNumber`[]\>

#### Implementation of

ChainProvider.getBalance

#### Defined in

[client/lib/Chain.ts:121](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L121)

___

### getBlockByHash

▸ `Abstract` **getBlockByHash**(`blockHash`, `includeTx?`): `Promise`<`Block`<`any`, `any`\>\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `blockHash` | `string` |  |
| `includeTx?` | `boolean` |  |

#### Returns

`Promise`<`Block`<`any`, `any`\>\>

#### Implementation of

ChainProvider.getBlockByHash

#### Defined in

[client/lib/Chain.ts:91](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L91)

___

### getBlockByNumber

▸ `Abstract` **getBlockByNumber**(`blockNumber?`, `includeTx?`): `Promise`<`Block`<`any`, `any`\>\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `blockNumber?` | `number` |  |
| `includeTx?` | `boolean` |  |

#### Returns

`Promise`<`Block`<`any`, `any`\>\>

#### Implementation of

ChainProvider.getBlockByNumber

#### Defined in

[client/lib/Chain.ts:100](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L100)

___

### getBlockHeight

▸ `Abstract` **getBlockHeight**(): `Promise`<`number`\>

#### Returns

`Promise`<`number`\>

#### Implementation of

ChainProvider.getBlockHeight

#### Defined in

[client/lib/Chain.ts:106](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L106)

___

### getFeeProvider

▸ **getFeeProvider**(): `Promise`<[`Fee`](chainify_client.Fee.md)\>

#### Returns

`Promise`<[`Fee`](chainify_client.Fee.md)\>

#### Defined in

[client/lib/Chain.ts:72](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L72)

___

### getFees

▸ `Abstract` **getFees**(`feeAsset?`): `Promise`<`FeeDetails`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `feeAsset?` | `Asset` |

#### Returns

`Promise`<`FeeDetails`\>

#### Defined in

[client/lib/Chain.ts:127](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L127)

___

### getNetwork

▸ **getNetwork**(): `N`

#### Returns

`N`

#### Defined in

[client/lib/Chain.ts:44](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L44)

___

### getProvider

▸ **getProvider**(): `T`

#### Returns

`T`

#### Defined in

[client/lib/Chain.ts:51](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L51)

___

### getTokenDetails

▸ **getTokenDetails**(`_asset`): `Promise`<`TokenDetails`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_asset` | `string` |

#### Returns

`Promise`<`TokenDetails`\>

#### Defined in

[client/lib/Chain.ts:79](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L79)

___

### getTransactionByHash

▸ `Abstract` **getTransactionByHash**(`txHash`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `txHash` | `string` |  |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Implementation of

ChainProvider.getTransactionByHash

#### Defined in

[client/lib/Chain.ts:115](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L115)

___

### sendRawTransaction

▸ `Abstract` **sendRawTransaction**(`rawTransaction`): `Promise`<`string`\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rawTransaction` | `string` |  |

#### Returns

`Promise`<`string`\>

#### Defined in

[client/lib/Chain.ts:136](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L136)

___

### sendRpcRequest

▸ `Abstract` **sendRpcRequest**(`method`, `params`): `Promise`<`any`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `method` | `string` |
| `params` | `any`[] |

#### Returns

`Promise`<`any`\>

#### Defined in

[client/lib/Chain.ts:143](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L143)

___

### setFeeProvider

▸ **setFeeProvider**(`feeProvider`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `feeProvider` | [`Fee`](chainify_client.Fee.md) |

#### Returns

`Promise`<`void`\>

#### Defined in

[client/lib/Chain.ts:65](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L65)

___

### setNetwork

▸ **setNetwork**(`network`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `network` | `N` |

#### Returns

`void`

#### Defined in

[client/lib/Chain.ts:37](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L37)

___

### setProvider

▸ **setProvider**(`provider`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `provider` | `T` |

#### Returns

`Promise`<`void`\>

#### Defined in

[client/lib/Chain.ts:58](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Chain.ts#L58)
