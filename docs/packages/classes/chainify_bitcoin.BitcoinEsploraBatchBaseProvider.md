---
id: "chainify_bitcoin.BitcoinEsploraBatchBaseProvider"
title: "Class: BitcoinEsploraBatchBaseProvider"
sidebar_label: "BitcoinEsploraBatchBaseProvider"
custom_edit_url: null
---

[@chainify/bitcoin](../modules/chainify_bitcoin.md).BitcoinEsploraBatchBaseProvider

## Hierarchy

- [`BitcoinEsploraBaseProvider`](chainify_bitcoin.BitcoinEsploraBaseProvider.md)

  ↳ **`BitcoinEsploraBatchBaseProvider`**

## Constructors

### constructor

• **new BitcoinEsploraBatchBaseProvider**(`options`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`EsploraBatchApiProviderOptions`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinEsploraTypes.EsploraBatchApiProviderOptions.md) |

#### Overrides

[BitcoinEsploraBaseProvider](chainify_bitcoin.BitcoinEsploraBaseProvider.md).[constructor](chainify_bitcoin.BitcoinEsploraBaseProvider.md#constructor)

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraBatchBaseProvider.ts:11](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraBatchBaseProvider.ts#L11)

## Properties

### \_options

• `Protected` **\_options**: [`EsploraApiProviderOptions`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinEsploraTypes.EsploraApiProviderOptions.md)

#### Inherited from

[BitcoinEsploraBaseProvider](chainify_bitcoin.BitcoinEsploraBaseProvider.md).[_options](chainify_bitcoin.BitcoinEsploraBaseProvider.md#_options)

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts:11](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts#L11)

___

### httpClient

• **httpClient**: `default`

#### Inherited from

[BitcoinEsploraBaseProvider](chainify_bitcoin.BitcoinEsploraBaseProvider.md).[httpClient](chainify_bitcoin.BitcoinEsploraBaseProvider.md#httpclient)

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts:10](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts#L10)

## Methods

### formatTransaction

▸ **formatTransaction**(`tx`, `currentHeight`): `Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `tx` | [`Transaction`](../namespaces/chainify_bitcoin.BitcoinTypes.BitcoinEsploraTypes.md#transaction) |
| `currentHeight` | `number` |

#### Returns

`Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Inherited from

[BitcoinEsploraBaseProvider](chainify_bitcoin.BitcoinEsploraBaseProvider.md).[formatTransaction](chainify_bitcoin.BitcoinEsploraBaseProvider.md#formattransaction)

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts:23](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts#L23)

___

### getAddressTransactionCounts

▸ **getAddressTransactionCounts**(`_addresses`): `Promise`<{ `[index: string]`: `number`;  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_addresses` | `AddressType`[] |

#### Returns

`Promise`<{ `[index: string]`: `number`;  }\>

#### Overrides

[BitcoinEsploraBaseProvider](chainify_bitcoin.BitcoinEsploraBaseProvider.md).[getAddressTransactionCounts](chainify_bitcoin.BitcoinEsploraBaseProvider.md#getaddresstransactioncounts)

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraBatchBaseProvider.ts:35](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraBatchBaseProvider.ts#L35)

___

### getFeePerByte

▸ **getFeePerByte**(`numberOfBlocks?`): `Promise`<`number`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `numberOfBlocks` | `number` |

#### Returns

`Promise`<`number`\>

#### Inherited from

[BitcoinEsploraBaseProvider](chainify_bitcoin.BitcoinEsploraBaseProvider.md).[getFeePerByte](chainify_bitcoin.BitcoinEsploraBaseProvider.md#getfeeperbyte)

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts:39](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts#L39)

___

### getMinRelayFee

▸ **getMinRelayFee**(): `Promise`<`number`\>

#### Returns

`Promise`<`number`\>

#### Inherited from

[BitcoinEsploraBaseProvider](chainify_bitcoin.BitcoinEsploraBaseProvider.md).[getMinRelayFee](chainify_bitcoin.BitcoinEsploraBaseProvider.md#getminrelayfee)

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts:72](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts#L72)

___

### getRawTransactionByHash

▸ **getRawTransactionByHash**(`transactionHash`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `transactionHash` | `string` |

#### Returns

`Promise`<`string`\>

#### Inherited from

[BitcoinEsploraBaseProvider](chainify_bitcoin.BitcoinEsploraBaseProvider.md).[getRawTransactionByHash](chainify_bitcoin.BitcoinEsploraBaseProvider.md#getrawtransactionbyhash)

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts:31](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts#L31)

___

### getTransactionHex

▸ **getTransactionHex**(`transactionHash`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `transactionHash` | `string` |

#### Returns

`Promise`<`string`\>

#### Inherited from

[BitcoinEsploraBaseProvider](chainify_bitcoin.BitcoinEsploraBaseProvider.md).[getTransactionHex](chainify_bitcoin.BitcoinEsploraBaseProvider.md#gettransactionhex)

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts:35](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts#L35)

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

[BitcoinEsploraBaseProvider](chainify_bitcoin.BitcoinEsploraBaseProvider.md).[getUnspentTransactions](chainify_bitcoin.BitcoinEsploraBaseProvider.md#getunspenttransactions)

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraBatchBaseProvider.ts:16](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraBatchBaseProvider.ts#L16)
