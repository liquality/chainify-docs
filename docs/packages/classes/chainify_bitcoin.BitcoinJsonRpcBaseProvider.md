---
id: "chainify_bitcoin.BitcoinJsonRpcBaseProvider"
title: "Class: BitcoinJsonRpcBaseProvider"
sidebar_label: "BitcoinJsonRpcBaseProvider"
custom_edit_url: null
---

[@chainify/bitcoin](../modules/chainify_bitcoin.md).BitcoinJsonRpcBaseProvider

## Hierarchy

- [`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md)

  ↳ **`BitcoinJsonRpcBaseProvider`**

## Constructors

### constructor

• **new BitcoinJsonRpcBaseProvider**(`options`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`ProviderOptions`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinJsonRpcTypes.ProviderOptions.md) |

#### Overrides

[BitcoinBaseChainProvider](chainify_bitcoin.BitcoinBaseChainProvider.md).[constructor](chainify_bitcoin.BitcoinBaseChainProvider.md#constructor)

#### Defined in

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts:12](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts#L12)

## Properties

### \_options

• `Protected` **\_options**: [`ProviderOptions`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinJsonRpcTypes.ProviderOptions.md)

#### Defined in

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts:10](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts#L10)

___

### jsonRpc

• **jsonRpc**: `default`

#### Defined in

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts:9](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts#L9)

## Methods

### formatTransaction

▸ **formatTransaction**(`tx`, `currentHeight`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `tx` | `any` |
| `currentHeight` | `number` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Overrides

[BitcoinBaseChainProvider](chainify_bitcoin.BitcoinBaseChainProvider.md).[formatTransaction](chainify_bitcoin.BitcoinBaseChainProvider.md#formattransaction)

#### Defined in

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts:22](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts#L22)

___

### getAddressTransactionCounts

▸ **getAddressTransactionCounts**(`_addresses`): `Promise`<[`AddressTxCounts`](../namespaces/chainify_bitcoin.BitcoinTypes.md#addresstxcounts)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_addresses` | `AddressType`[] |

#### Returns

`Promise`<[`AddressTxCounts`](../namespaces/chainify_bitcoin.BitcoinTypes.md#addresstxcounts)\>

#### Overrides

[BitcoinBaseChainProvider](chainify_bitcoin.BitcoinBaseChainProvider.md).[getAddressTransactionCounts](chainify_bitcoin.BitcoinBaseChainProvider.md#getaddresstransactioncounts)

#### Defined in

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts:58](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts#L58)

___

### getFeePerByte

▸ **getFeePerByte**(`numberOfBlocks?`): `Promise`<`number`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `numberOfBlocks?` | `number` |

#### Returns

`Promise`<`number`\>

#### Overrides

[BitcoinBaseChainProvider](chainify_bitcoin.BitcoinBaseChainProvider.md).[getFeePerByte](chainify_bitcoin.BitcoinBaseChainProvider.md#getfeeperbyte)

#### Defined in

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts:38](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts#L38)

___

### getMinRelayFee

▸ **getMinRelayFee**(): `Promise`<`number`\>

#### Returns

`Promise`<`number`\>

#### Overrides

[BitcoinBaseChainProvider](chainify_bitcoin.BitcoinBaseChainProvider.md).[getMinRelayFee](chainify_bitcoin.BitcoinBaseChainProvider.md#getminrelayfee)

#### Defined in

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts:69](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts#L69)

___

### getRawTransactionByHash

▸ **getRawTransactionByHash**(`transactionHash`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `transactionHash` | `string` |

#### Returns

`Promise`<`string`\>

#### Overrides

[BitcoinBaseChainProvider](chainify_bitcoin.BitcoinBaseChainProvider.md).[getRawTransactionByHash](chainify_bitcoin.BitcoinBaseChainProvider.md#getrawtransactionbyhash)

#### Defined in

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts:30](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts#L30)

___

### getTransactionHex

▸ **getTransactionHex**(`transactionHash`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `transactionHash` | `string` |

#### Returns

`Promise`<`string`\>

#### Overrides

[BitcoinBaseChainProvider](chainify_bitcoin.BitcoinBaseChainProvider.md).[getTransactionHex](chainify_bitcoin.BitcoinBaseChainProvider.md#gettransactionhex)

#### Defined in

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts:34](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts#L34)

___

### getUnspentTransactions

▸ **getUnspentTransactions**(`_addresses`): `Promise`<[`UTXO`](../interfaces/chainify_bitcoin.BitcoinTypes.UTXO.md)[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_addresses` | `AddressType`[] |

#### Returns

`Promise`<[`UTXO`](../interfaces/chainify_bitcoin.BitcoinTypes.UTXO.md)[]\>

#### Overrides

[BitcoinBaseChainProvider](chainify_bitcoin.BitcoinBaseChainProvider.md).[getUnspentTransactions](chainify_bitcoin.BitcoinBaseChainProvider.md#getunspenttransactions)

#### Defined in

[bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts:52](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/jsonRpc/BitcoinJsonRpcBaseProvider.ts#L52)
