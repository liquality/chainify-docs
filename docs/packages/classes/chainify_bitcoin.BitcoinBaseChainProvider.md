---
id: "chainify_bitcoin.BitcoinBaseChainProvider"
title: "Class: BitcoinBaseChainProvider"
sidebar_label: "BitcoinBaseChainProvider"
custom_edit_url: null
---

[@chainify/bitcoin](../modules/chainify_bitcoin.md).BitcoinBaseChainProvider

## Hierarchy

- **`BitcoinBaseChainProvider`**

  ↳ [`BitcoinEsploraBaseProvider`](chainify_bitcoin.BitcoinEsploraBaseProvider.md)

  ↳ [`BitcoinJsonRpcBaseProvider`](chainify_bitcoin.BitcoinJsonRpcBaseProvider.md)

## Constructors

### constructor

• **new BitcoinBaseChainProvider**()

## Methods

### formatTransaction

▸ `Abstract` **formatTransaction**(`tx`, `currentHeight`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `tx` | `any` |
| `currentHeight` | `number` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Defined in

[bitcoin/lib/chain/BitcoinBaseChainProvider.ts:5](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/BitcoinBaseChainProvider.ts#L5)

___

### getAddressTransactionCounts

▸ `Abstract` **getAddressTransactionCounts**(`_addresses`): `Promise`<[`AddressTxCounts`](../namespaces/chainify_bitcoin.BitcoinTypes.md#addresstxcounts)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_addresses` | `AddressType`[] |

#### Returns

`Promise`<[`AddressTxCounts`](../namespaces/chainify_bitcoin.BitcoinTypes.md#addresstxcounts)\>

#### Defined in

[bitcoin/lib/chain/BitcoinBaseChainProvider.ts:15](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/BitcoinBaseChainProvider.ts#L15)

___

### getFeePerByte

▸ `Abstract` **getFeePerByte**(`numberOfBlocks?`): `Promise`<`number`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `numberOfBlocks?` | `number` |

#### Returns

`Promise`<`number`\>

#### Defined in

[bitcoin/lib/chain/BitcoinBaseChainProvider.ts:11](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/BitcoinBaseChainProvider.ts#L11)

___

### getMinRelayFee

▸ `Abstract` **getMinRelayFee**(): `Promise`<`number`\>

#### Returns

`Promise`<`number`\>

#### Defined in

[bitcoin/lib/chain/BitcoinBaseChainProvider.ts:17](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/BitcoinBaseChainProvider.ts#L17)

___

### getRawTransactionByHash

▸ `Abstract` **getRawTransactionByHash**(`transactionHash`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `transactionHash` | `string` |

#### Returns

`Promise`<`string`\>

#### Defined in

[bitcoin/lib/chain/BitcoinBaseChainProvider.ts:7](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/BitcoinBaseChainProvider.ts#L7)

___

### getTransactionHex

▸ `Abstract` **getTransactionHex**(`transactionHash`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `transactionHash` | `string` |

#### Returns

`Promise`<`string`\>

#### Defined in

[bitcoin/lib/chain/BitcoinBaseChainProvider.ts:9](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/BitcoinBaseChainProvider.ts#L9)

___

### getUnspentTransactions

▸ `Abstract` **getUnspentTransactions**(`addresses`): `Promise`<[`UTXO`](../interfaces/chainify_bitcoin.BitcoinTypes.UTXO.md)[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `addresses` | `AddressType`[] |

#### Returns

`Promise`<[`UTXO`](../interfaces/chainify_bitcoin.BitcoinTypes.UTXO.md)[]\>

#### Defined in

[bitcoin/lib/chain/BitcoinBaseChainProvider.ts:13](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/chain/BitcoinBaseChainProvider.ts#L13)
