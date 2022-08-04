---
id: "chainify_bitcoin.BitcoinTypes"
title: "Namespace: BitcoinTypes"
sidebar_label: "BitcoinTypes"
custom_edit_url: null
---

[@chainify/bitcoin](../modules/chainify_bitcoin.md).BitcoinTypes

## Namespaces

- [BitcoinEsploraTypes](chainify_bitcoin.BitcoinTypes.BitcoinEsploraTypes.md)
- [BitcoinJsonRpcTypes](chainify_bitcoin.BitcoinTypes.BitcoinJsonRpcTypes.md)

## Enumerations

- [AddressType](../enums/chainify_bitcoin.BitcoinTypes.AddressType.md)
- [SwapMode](../enums/chainify_bitcoin.BitcoinTypes.SwapMode.md)

## Interfaces

- [BitcoinHDWalletProviderOptions](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinHDWalletProviderOptions.md)
- [BitcoinNetwork](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinNetwork.md)
- [BitcoinNodeWalletOptions](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinNodeWalletOptions.md)
- [BitcoinSwapProviderOptions](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinSwapProviderOptions.md)
- [BitcoinWalletProviderOptions](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinWalletProviderOptions.md)
- [Input](../interfaces/chainify_bitcoin.BitcoinTypes.Input.md)
- [Output](../interfaces/chainify_bitcoin.BitcoinTypes.Output.md)
- [OutputTarget](../interfaces/chainify_bitcoin.BitcoinTypes.OutputTarget.md)
- [P2SHInput](../interfaces/chainify_bitcoin.BitcoinTypes.P2SHInput.md)
- [PsbtInputTarget](../interfaces/chainify_bitcoin.BitcoinTypes.PsbtInputTarget.md)
- [ScriptPubKey](../interfaces/chainify_bitcoin.BitcoinTypes.ScriptPubKey.md)
- [Transaction](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)
- [UTXO](../interfaces/chainify_bitcoin.BitcoinTypes.UTXO.md)

## Type aliases

### AddressTxCounts

Ƭ **AddressTxCounts**: `Object`

#### Index signature

▪ [index: `string`]: `number`

#### Defined in

[bitcoin/lib/types.ts:88](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/types.ts#L88)

___

### PaymentVariants

Ƭ **PaymentVariants**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `p2sh?` | `payments.Payment` |
| `p2shSegwit?` | `payments.Payment` |
| `p2wsh?` | `payments.Payment` |

#### Defined in

[bitcoin/lib/swap/types.ts:13](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/types.ts#L13)

___

### TransactionMatchesFunction

Ƭ **TransactionMatchesFunction**: (`tx`: `Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>) => `boolean`

#### Type declaration

▸ (`tx`): `boolean`

##### Parameters

| Name | Type |
| :------ | :------ |
| `tx` | `Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\> |

##### Returns

`boolean`

#### Defined in

[bitcoin/lib/swap/types.ts:11](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/swap/types.ts#L11)
