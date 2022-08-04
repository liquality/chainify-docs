---
id: "chainify_bitcoin.BitcoinJsonRpcProvider"
title: "Class: BitcoinJsonRpcProvider"
sidebar_label: "BitcoinJsonRpcProvider"
custom_edit_url: null
---

[@chainify/bitcoin](../modules/chainify_bitcoin.md).BitcoinJsonRpcProvider

## Hierarchy

- `default`<[`BitcoinJsonRpcBaseProvider`](chainify_bitcoin.BitcoinJsonRpcBaseProvider.md)\>

  ↳ **`BitcoinJsonRpcProvider`**

## Constructors

### constructor

• **new BitcoinJsonRpcProvider**(`options`, `feeProvider?`, `feeOptions?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`ProviderOptions`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinJsonRpcTypes.ProviderOptions.md) |
| `feeProvider?` | `default` |
| `feeOptions?` | [`FeeOptions`](../namespaces/chainify_bitcoin.BitcoinTypes.BitcoinJsonRpcTypes.md#feeoptions) |

#### Overrides

Chain&lt;BitcoinJsonRpcBaseProvider\&gt;.constructor

#### Defined in

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts:14](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts#L14)

## Properties

### feeProvider

• `Protected` **feeProvider**: `default`

#### Inherited from

Chain.feeProvider

#### Defined in

client/dist/lib/Chain.d.ts:11

___

### jsonRpc

• **jsonRpc**: `default`

#### Defined in

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts:11](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts#L11)

___

### network

• `Protected` **network**: `Network`

#### Inherited from

Chain.network

#### Defined in

client/dist/lib/Chain.d.ts:12

___

### provider

• `Protected` **provider**: [`BitcoinJsonRpcBaseProvider`](chainify_bitcoin.BitcoinJsonRpcBaseProvider.md)

#### Inherited from

Chain.provider

#### Defined in

client/dist/lib/Chain.d.ts:13

## Methods

### getBalance

▸ **getBalance**(`_addresses`, `_assets`): `Promise`<`BigNumber`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_addresses` | `AddressType`[] |
| `_assets` | `Asset`[] |

#### Returns

`Promise`<`BigNumber`[]\>

#### Overrides

Chain.getBalance

#### Defined in

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts:107](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts#L107)

___

### getBlockByHash

▸ **getBlockByHash**(`blockHash`, `includeTx?`): `Promise`<`Block`<`any`, `any`\>\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `blockHash` | `string` | `undefined` |
| `includeTx` | `boolean` | `false` |

#### Returns

`Promise`<`Block`<`any`, `any`\>\>

#### Overrides

Chain.getBlockByHash

#### Defined in

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts:20](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts#L20)

___

### getBlockByNumber

▸ **getBlockByNumber**(`blockNumber?`, `includeTx?`): `Promise`<`Block`<`any`, `any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `blockNumber?` | `number` |
| `includeTx?` | `boolean` |

#### Returns

`Promise`<`Block`<`any`, `any`\>\>

#### Overrides

Chain.getBlockByNumber

#### Defined in

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts:66](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts#L66)

___

### getBlockHeight

▸ **getBlockHeight**(): `Promise`<`number`\>

#### Returns

`Promise`<`number`\>

#### Overrides

Chain.getBlockHeight

#### Defined in

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts:88](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts#L88)

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

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts:114](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts#L114)

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

▸ **getProvider**(): [`BitcoinJsonRpcBaseProvider`](chainify_bitcoin.BitcoinJsonRpcBaseProvider.md)

#### Returns

[`BitcoinJsonRpcBaseProvider`](chainify_bitcoin.BitcoinJsonRpcBaseProvider.md)

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

▸ **getTransactionByHash**(`txHash`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txHash` | `string` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Overrides

Chain.getTransactionByHash

#### Defined in

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts:92](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts#L92)

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

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts:132](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts#L132)

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

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts:136](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcProvider.ts#L136)

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
| `provider` | [`BitcoinJsonRpcBaseProvider`](chainify_bitcoin.BitcoinJsonRpcBaseProvider.md) |

#### Returns

`Promise`<`void`\>

#### Inherited from

Chain.setProvider

#### Defined in

client/dist/lib/Chain.d.ts:30
