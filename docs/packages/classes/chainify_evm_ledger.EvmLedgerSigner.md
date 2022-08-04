---
id: "chainify_evm_ledger.EvmLedgerSigner"
title: "Class: EvmLedgerSigner"
sidebar_label: "EvmLedgerSigner"
custom_edit_url: null
---

[@chainify/evm-ledger](../modules/chainify_evm_ledger.md).EvmLedgerSigner

## Hierarchy

- `Signer`

  ↳ **`EvmLedgerSigner`**

## Constructors

### constructor

• **new EvmLedgerSigner**(`getApp`, `derivationPath?`, `provider?`, `addressCache?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `getApp` | [`GetAppType`](../namespaces/chainify_evm_ledger.EvmLedgerProviderTypes.md#getapptype) |
| `derivationPath?` | `string` |
| `provider?` | `Provider` |
| `addressCache?` | `Address` |

#### Overrides

Signer.constructor

#### Defined in

[evm-ledger/lib/EvmLedgerSigner.ts:44](https://github.com/liquality/chainify/blob/540cfa69/packages/evm-ledger/lib/EvmLedgerSigner.ts#L44)

## Properties

### provider

• **provider**: `Provider`

#### Overrides

Signer.provider

#### Defined in

[evm-ledger/lib/EvmLedgerSigner.ts:38](https://github.com/liquality/chainify/blob/540cfa69/packages/evm-ledger/lib/EvmLedgerSigner.ts#L38)

## Methods

### connect

▸ **connect**(`provider`): [`EvmLedgerSigner`](chainify_evm_ledger.EvmLedgerSigner.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `provider` | `Provider` |

#### Returns

[`EvmLedgerSigner`](chainify_evm_ledger.EvmLedgerSigner.md)

#### Overrides

Signer.connect

#### Defined in

[evm-ledger/lib/EvmLedgerSigner.ts:108](https://github.com/liquality/chainify/blob/540cfa69/packages/evm-ledger/lib/EvmLedgerSigner.ts#L108)

___

### getAddress

▸ **getAddress**(): `Promise`<`string`\>

#### Returns

`Promise`<`string`\>

#### Overrides

Signer.getAddress

#### Defined in

[evm-ledger/lib/EvmLedgerSigner.ts:58](https://github.com/liquality/chainify/blob/540cfa69/packages/evm-ledger/lib/EvmLedgerSigner.ts#L58)

___

### signMessage

▸ **signMessage**(`message`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` \| `Bytes` |

#### Returns

`Promise`<`string`\>

#### Overrides

Signer.signMessage

#### Defined in

[evm-ledger/lib/EvmLedgerSigner.ts:67](https://github.com/liquality/chainify/blob/540cfa69/packages/evm-ledger/lib/EvmLedgerSigner.ts#L67)

___

### signTransaction

▸ **signTransaction**(`transaction`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `transaction` | `TransactionRequest` |

#### Returns

`Promise`<`string`\>

#### Overrides

Signer.signTransaction

#### Defined in

[evm-ledger/lib/EvmLedgerSigner.ts:80](https://github.com/liquality/chainify/blob/540cfa69/packages/evm-ledger/lib/EvmLedgerSigner.ts#L80)
