---
id: "chainify_bitcoin.BitcoinUtils"
title: "Namespace: BitcoinUtils"
sidebar_label: "BitcoinUtils"
custom_edit_url: null
---

[@chainify/bitcoin](../modules/chainify_bitcoin.md).BitcoinUtils

## Type aliases

### CoinSelectTarget

Ƭ **CoinSelectTarget**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `id?` | `string` |
| `script?` | `Buffer` |
| `value` | `number` |

#### Defined in

[bitcoin/lib/utils.ts:30](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/utils.ts#L30)

## Variables

### AddressTypes

• `Const` **AddressTypes**: `string`[]

#### Defined in

[bitcoin/lib/utils.ts:10](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/utils.ts#L10)

## Functions

### calculateFee

▸ **calculateFee**(`numInputs`, `numOutputs`, `feePerByte`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `numInputs` | `number` |
| `numOutputs` | `number` |
| `feePerByte` | `number` |

#### Returns

`number`

#### Defined in

[bitcoin/lib/utils.ts:12](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/utils.ts#L12)

___

### compressPubKey

▸ **compressPubKey**(`pubKey`): `string`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pubKey` | `string` |  |

#### Returns

`string`

#### Defined in

[bitcoin/lib/utils.ts:21](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/utils.ts#L21)

___

### decodeRawTransaction

▸ **decodeRawTransaction**(`hex`, `network`): [`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `hex` | `string` |
| `network` | [`BitcoinNetwork`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinNetwork.md) |

#### Returns

[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)

#### Defined in

[bitcoin/lib/utils.ts:74](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/utils.ts#L74)

___

### getPubKeyHash

▸ **getPubKeyHash**(`address`, `network`): `Buffer`

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `network` | [`BitcoinNetwork`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinNetwork.md) |

#### Returns

`Buffer`

#### Defined in

[bitcoin/lib/utils.ts:194](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/utils.ts#L194)

___

### normalizeTransactionObject

▸ **normalizeTransactionObject**(`tx`, `fee`, `block?`): `Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `tx` | [`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md) |
| `fee` | `number` |
| `block?` | `Object` |
| `block.hash` | `string` |
| `block.number` | `number` |

#### Returns

`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>

#### Defined in

[bitcoin/lib/utils.ts:129](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/utils.ts#L129)

___

### selectCoins

▸ **selectCoins**(`utxos`, `targets`, `feePerByte`, `fixedInputs?`): `Object`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `utxos` | [`UTXO`](../interfaces/chainify_bitcoin.BitcoinTypes.UTXO.md)[] | `undefined` |
| `targets` | [`CoinSelectTarget`](chainify_bitcoin.BitcoinUtils.md#coinselecttarget)[] | `undefined` |
| `feePerByte` | `number` | `undefined` |
| `fixedInputs` | [`UTXO`](../interfaces/chainify_bitcoin.BitcoinTypes.UTXO.md)[] | `[]` |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `change` | [`CoinSelectTarget`](chainify_bitcoin.BitcoinUtils.md#coinselecttarget) |
| `fee` | `number` |
| `inputs` | [`UTXO`](../interfaces/chainify_bitcoin.BitcoinTypes.UTXO.md)[] |
| `outputs` | [`CoinSelectTarget`](chainify_bitcoin.BitcoinUtils.md#coinselecttarget)[] |

#### Defined in

[bitcoin/lib/utils.ts:45](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/utils.ts#L45)

___

### validateAddress

▸ **validateAddress**(`_address`, `network`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `_address` | `AddressType` |
| `network` | [`BitcoinNetwork`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinNetwork.md) |

#### Returns

`void`

#### Defined in

[bitcoin/lib/utils.ts:210](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/utils.ts#L210)

___

### witnessStackToScriptWitness

▸ **witnessStackToScriptWitness**(`witness`): `Buffer`

#### Parameters

| Name | Type |
| :------ | :------ |
| `witness` | `Buffer`[] |

#### Returns

`Buffer`

#### Defined in

[bitcoin/lib/utils.ts:164](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/utils.ts#L164)
