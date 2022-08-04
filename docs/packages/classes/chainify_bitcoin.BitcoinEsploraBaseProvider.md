---
id: "chainify_bitcoin.BitcoinEsploraBaseProvider"
title: "Class: BitcoinEsploraBaseProvider"
sidebar_label: "BitcoinEsploraBaseProvider"
custom_edit_url: null
---

[@chainify/bitcoin](../modules/chainify_bitcoin.md).BitcoinEsploraBaseProvider

## Hierarchy

- [`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md)

  ↳ **`BitcoinEsploraBaseProvider`**

  ↳↳ [`BitcoinEsploraBatchBaseProvider`](chainify_bitcoin.BitcoinEsploraBatchBaseProvider.md)

## Constructors

### constructor

• **new BitcoinEsploraBaseProvider**(`options`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`EsploraApiProviderOptions`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinEsploraTypes.EsploraApiProviderOptions.md) |

#### Overrides

[BitcoinBaseChainProvider](chainify_bitcoin.BitcoinBaseChainProvider.md).[constructor](chainify_bitcoin.BitcoinBaseChainProvider.md#constructor)

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts:13](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts#L13)

## Properties

### \_options

• `Protected` **\_options**: [`EsploraApiProviderOptions`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinEsploraTypes.EsploraApiProviderOptions.md)

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts:11](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts#L11)

___

### httpClient

• **httpClient**: `default`

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

#### Overrides

[BitcoinBaseChainProvider](chainify_bitcoin.BitcoinBaseChainProvider.md).[formatTransaction](chainify_bitcoin.BitcoinBaseChainProvider.md#formattransaction)

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts:23](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts#L23)

___

### getAddressTransactionCounts

▸ **getAddressTransactionCounts**(`_addresses`): `Promise`<`any`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_addresses` | `AddressType`[] |

#### Returns

`Promise`<`any`\>

#### Overrides

[BitcoinBaseChainProvider](chainify_bitcoin.BitcoinBaseChainProvider.md).[getAddressTransactionCounts](chainify_bitcoin.BitcoinBaseChainProvider.md#getaddresstransactioncounts)

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts:60](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts#L60)

___

### getFeePerByte

▸ **getFeePerByte**(`numberOfBlocks?`): `Promise`<`number`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `numberOfBlocks` | `number` |

#### Returns

`Promise`<`number`\>

#### Overrides

[BitcoinBaseChainProvider](chainify_bitcoin.BitcoinBaseChainProvider.md).[getFeePerByte](chainify_bitcoin.BitcoinBaseChainProvider.md#getfeeperbyte)

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts:39](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts#L39)

___

### getMinRelayFee

▸ **getMinRelayFee**(): `Promise`<`number`\>

#### Returns

`Promise`<`number`\>

#### Overrides

[BitcoinBaseChainProvider](chainify_bitcoin.BitcoinBaseChainProvider.md).[getMinRelayFee](chainify_bitcoin.BitcoinBaseChainProvider.md#getminrelayfee)

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

#### Overrides

[BitcoinBaseChainProvider](chainify_bitcoin.BitcoinBaseChainProvider.md).[getRawTransactionByHash](chainify_bitcoin.BitcoinBaseChainProvider.md#getrawtransactionbyhash)

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

#### Overrides

[BitcoinBaseChainProvider](chainify_bitcoin.BitcoinBaseChainProvider.md).[getTransactionHex](chainify_bitcoin.BitcoinBaseChainProvider.md#gettransactionhex)

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

[BitcoinBaseChainProvider](chainify_bitcoin.BitcoinBaseChainProvider.md).[getUnspentTransactions](chainify_bitcoin.BitcoinBaseChainProvider.md#getunspenttransactions)

#### Defined in

[bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts:53](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/BitcoinEsploraBaseProvider.ts#L53)
