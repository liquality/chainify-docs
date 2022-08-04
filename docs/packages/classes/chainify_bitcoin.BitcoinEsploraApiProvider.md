---
id: "chainify_bitcoin.BitcoinEsploraApiProvider"
title: "Class: BitcoinEsploraApiProvider"
sidebar_label: "BitcoinEsploraApiProvider"
custom_edit_url: null
---

[@chainify/bitcoin](../modules/chainify_bitcoin.md).BitcoinEsploraApiProvider

## Hierarchy

- `default`<[`BitcoinEsploraBaseProvider`](chainify_bitcoin.BitcoinEsploraBaseProvider.md)\>

  ↳ **`BitcoinEsploraApiProvider`**

## Constructors

### constructor

• **new BitcoinEsploraApiProvider**(`options`, `provider?`, `feeProvider?`, `feeOptions?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`EsploraBatchApiProviderOptions`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinEsploraTypes.EsploraBatchApiProviderOptions.md) |
| `provider?` | [`BitcoinEsploraBaseProvider`](chainify_bitcoin.BitcoinEsploraBaseProvider.md) |
| `feeProvider?` | `default` |
| `feeOptions?` | [`FeeOptions`](../namespaces/chainify_bitcoin.BitcoinTypes.BitcoinEsploraTypes.md#feeoptions) |

#### Overrides

Chain&lt;BitcoinEsploraBaseProvider\&gt;.constructor

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts:13](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts#L13)

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

• `Protected` **provider**: [`BitcoinEsploraBaseProvider`](chainify_bitcoin.BitcoinEsploraBaseProvider.md)

#### Inherited from

Chain.provider

#### Defined in

client/dist/lib/Chain.d.ts:13

## Methods

### getBalance

▸ **getBalance**(`_addresses`): `Promise`<`BigNumber`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_addresses` | `AddressType`[] |

#### Returns

`Promise`<`BigNumber`[]\>

#### Overrides

Chain.getBalance

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts:70](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts#L70)

___

### getBlockByHash

▸ **getBlockByHash**(`blockHash`): `Promise`<`Block`<`any`, `any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `blockHash` | `string` |

#### Returns

`Promise`<`Block`<`any`, `any`\>\>

#### Overrides

Chain.getBlockByHash

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts:25](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts#L25)

___

### getBlockByNumber

▸ **getBlockByNumber**(`blockNumber?`): `Promise`<`Block`<`any`, `any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `blockNumber?` | `number` |

#### Returns

`Promise`<`Block`<`any`, `any`\>\>

#### Overrides

Chain.getBlockByNumber

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts:54](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts#L54)

___

### getBlockHeight

▸ **getBlockHeight**(): `Promise`<`number`\>

#### Returns

`Promise`<`number`\>

#### Overrides

Chain.getBlockHeight

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts:61](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts#L61)

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

[bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts:77](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts#L77)

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

▸ **getProvider**(): [`BitcoinEsploraBaseProvider`](chainify_bitcoin.BitcoinEsploraBaseProvider.md)

#### Returns

[`BitcoinEsploraBaseProvider`](chainify_bitcoin.BitcoinEsploraBaseProvider.md)

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

[bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts:66](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts#L66)

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

[bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts:95](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts#L95)

___

### sendRpcRequest

▸ **sendRpcRequest**(`_method`, `_params`): `Promise`<`any`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_method` | `string` |
| `_params` | `any`[] |

#### Returns

`Promise`<`any`\>

#### Overrides

Chain.sendRpcRequest

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts:99](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraApiProvider.ts#L99)

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
| `provider` | [`BitcoinEsploraBaseProvider`](chainify_bitcoin.BitcoinEsploraBaseProvider.md) |

#### Returns

`Promise`<`void`\>

#### Inherited from

Chain.setProvider

#### Defined in

client/dist/lib/Chain.d.ts:30
