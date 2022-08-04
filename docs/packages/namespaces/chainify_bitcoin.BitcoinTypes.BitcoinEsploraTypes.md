---
id: "chainify_bitcoin.BitcoinTypes.BitcoinEsploraTypes"
title: "Namespace: BitcoinEsploraTypes"
sidebar_label: "BitcoinEsploraTypes"
custom_edit_url: null
---

[@chainify/bitcoin](../modules/chainify_bitcoin.md).[BitcoinTypes](chainify_bitcoin.BitcoinTypes.md).BitcoinEsploraTypes

## Interfaces

- [EsploraApiProviderOptions](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinEsploraTypes.EsploraApiProviderOptions.md)
- [EsploraBatchApiProviderOptions](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinEsploraTypes.EsploraBatchApiProviderOptions.md)

## Type aliases

### Address

Ƭ **Address**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `chain_stats` | { `funded_txo_count`: `number` ; `funded_txo_sum`: `number` ; `spent_txo_count`: `number` ; `spent_txo_sum`: `number` ; `tx_count`: `number`  } |
| `chain_stats.funded_txo_count` | `number` |
| `chain_stats.funded_txo_sum` | `number` |
| `chain_stats.spent_txo_count` | `number` |
| `chain_stats.spent_txo_sum` | `number` |
| `chain_stats.tx_count` | `number` |
| `mempool_stats` | { `funded_txo_count`: `number` ; `funded_txo_sum`: `number` ; `spent_txo_count`: `number` ; `spent_txo_sum`: `number` ; `tx_count`: `number`  } |
| `mempool_stats.funded_txo_count` | `number` |
| `mempool_stats.funded_txo_sum` | `number` |
| `mempool_stats.spent_txo_count` | `number` |
| `mempool_stats.spent_txo_sum` | `number` |
| `mempool_stats.tx_count` | `number` |

#### Defined in

[bitcoin/lib/chain/esplora/types.ts:19](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/types.ts#L19)

___

### BatchUTXOs

Ƭ **BatchUTXOs**: { `address`: `string` ; `utxo`: [`UTXO`](chainify_bitcoin.BitcoinTypes.BitcoinEsploraTypes.md#utxo)[]  }[]

#### Defined in

[bitcoin/lib/chain/esplora/types.ts:83](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/types.ts#L83)

___

### Block

Ƭ **Block**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `bits` | `number` |
| `difficulty` | `number` |
| `height` | `number` |
| `id` | `string` |
| `mediantime` | `number` |
| `merlke_root` | `string` |
| `nonce` | `number` |
| `previousblockhash` | `string` |
| `size` | `number` |
| `timestamp` | `number` |
| `tx_count` | `number` |
| `version` | `number` |
| `weight` | `number` |

#### Defined in

[bitcoin/lib/chain/esplora/types.ts:67](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/types.ts#L67)

___

### FeeEstimates

Ƭ **FeeEstimates**: `Object`

#### Index signature

▪ [index: `string`]: `number`

#### Defined in

[bitcoin/lib/chain/esplora/types.ts:3](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/types.ts#L3)

___

### FeeOptions

Ƭ **FeeOptions**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `averageTargetBlocks?` | `number` |
| `fastTargetBlocks?` | `number` |
| `slowTargetBlocks?` | `number` |

#### Defined in

[bitcoin/lib/chain/esplora/types.ts:96](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/types.ts#L96)

___

### Transaction

Ƭ **Transaction**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `fee` | `number` |
| `locktime` | `number` |
| `size` | `number` |
| `status` | [`TxStatus`](chainify_bitcoin.BitcoinTypes.BitcoinEsploraTypes.md#txstatus) |
| `txid` | `string` |
| `version` | `number` |
| `vin` | [`Vin`](chainify_bitcoin.BitcoinTypes.BitcoinEsploraTypes.md#vin)[] |
| `vout` | [`Vout`](chainify_bitcoin.BitcoinTypes.BitcoinEsploraTypes.md#vout)[] |
| `weight` | `number` |

#### Defined in

[bitcoin/lib/chain/esplora/types.ts:55](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/types.ts#L55)

___

### TxStatus

Ƭ **TxStatus**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `block_hash?` | `string` |
| `block_height?` | `number` |
| `block_time?` | `number` |
| `confirmed` | `boolean` |

#### Defined in

[bitcoin/lib/chain/esplora/types.ts:5](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/types.ts#L5)

___

### UTXO

Ƭ **UTXO**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `status` | [`TxStatus`](chainify_bitcoin.BitcoinTypes.BitcoinEsploraTypes.md#txstatus) |
| `txid` | `string` |
| `value` | `number` |
| `vout` | `number` |

#### Defined in

[bitcoin/lib/chain/esplora/types.ts:12](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/types.ts#L12)

___

### Vin

Ƭ **Vin**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `is_coinbase` | `boolean` |
| `prevout` | [`Vout`](chainify_bitcoin.BitcoinTypes.BitcoinEsploraTypes.md#vout) |
| `scriptsig` | `string` |
| `scriptsig_asm` | `string` |
| `sequence` | `number` |
| `txid` | `string` |
| `vout` | `number` |

#### Defined in

[bitcoin/lib/chain/esplora/types.ts:45](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/types.ts#L45)

___

### Vout

Ƭ **Vout**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `scriptpubkey` | `string` |
| `scriptpubkey_address?` | `string` |
| `scriptpubkey_asm` | `string` |
| `scriptpubkey_type` | `string` |
| `value` | `number` |

#### Defined in

[bitcoin/lib/chain/esplora/types.ts:37](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/esplora/types.ts#L37)
