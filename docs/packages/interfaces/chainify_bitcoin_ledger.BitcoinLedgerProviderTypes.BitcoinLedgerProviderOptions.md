---
id: "chainify_bitcoin_ledger.BitcoinLedgerProviderTypes.BitcoinLedgerProviderOptions"
title: "Interface: BitcoinLedgerProviderOptions"
sidebar_label: "BitcoinLedgerProviderOptions"
custom_edit_url: null
---

[@chainify/bitcoin-ledger](../modules/chainify_bitcoin_ledger.md).[BitcoinLedgerProviderTypes](../namespaces/chainify_bitcoin_ledger.BitcoinLedgerProviderTypes.md).BitcoinLedgerProviderOptions

## Hierarchy

- `CreateOptions`

  ↳ **`BitcoinLedgerProviderOptions`**

## Properties

### addressType

• **addressType**: `AddressType`

#### Defined in

[bitcoin-ledger/lib/types.ts:8](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/types.ts#L8)

___

### baseChainCode

• `Optional` **baseChainCode**: `string`

#### Defined in

[bitcoin-ledger/lib/types.ts:7](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/types.ts#L7)

___

### baseDerivationPath

• **baseDerivationPath**: `string`

#### Defined in

[bitcoin-ledger/lib/types.ts:5](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/types.ts#L5)

___

### basePublicKey

• `Optional` **basePublicKey**: `string`

#### Defined in

[bitcoin-ledger/lib/types.ts:6](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/types.ts#L6)

___

### network

• **network**: `BitcoinNetwork`

#### Overrides

LedgerProviderTypes.CreateOptions.network

#### Defined in

[bitcoin-ledger/lib/types.ts:9](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/types.ts#L9)

___

### scrambleKey

• `Optional` **scrambleKey**: `string`

#### Inherited from

LedgerProviderTypes.CreateOptions.scrambleKey

#### Defined in

hw-ledger/dist/lib/types.d.ts:8

___

### transportCreator

• **transportCreator**: `TransportCreator`

#### Inherited from

LedgerProviderTypes.CreateOptions.transportCreator

#### Defined in

hw-ledger/dist/lib/types.d.ts:6
