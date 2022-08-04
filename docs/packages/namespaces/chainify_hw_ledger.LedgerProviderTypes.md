---
id: "chainify_hw_ledger.LedgerProviderTypes"
title: "Namespace: LedgerProviderTypes"
sidebar_label: "LedgerProviderTypes"
custom_edit_url: null
---

[@chainify/hw-ledger](../modules/chainify_hw_ledger.md).LedgerProviderTypes

## Interfaces

- [CreateOptions](../interfaces/chainify_hw_ledger.LedgerProviderTypes.CreateOptions.md)
- [TransportCreator](../interfaces/chainify_hw_ledger.LedgerProviderTypes.TransportCreator.md)

## Type aliases

### GetAddressesFuncType

Ƭ **GetAddressesFuncType**: (`start?`: `number`, `numAddresses?`: `number`, `change?`: `boolean`) => `Promise`<`Address`[]\>

#### Type declaration

▸ (`start?`, `numAddresses?`, `change?`): `Promise`<`Address`[]\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `start?` | `number` |
| `numAddresses?` | `number` |
| `change?` | `boolean` |

##### Returns

`Promise`<`Address`[]\>

#### Defined in

[hw-ledger/lib/types.ts:15](https://github.com/liquality/chainify/blob/540cfa69/packages/hw-ledger/lib/types.ts#L15)

___

### HWApp

Ƭ **HWApp**: `HwAppBitcoin` \| `HwAppEthereum`

#### Defined in

[hw-ledger/lib/types.ts:12](https://github.com/liquality/chainify/blob/540cfa69/packages/hw-ledger/lib/types.ts#L12)

___

### Newable

Ƭ **Newable**<`T`\>: `Object`

#### Type parameters

| Name |
| :------ |
| `T` |

#### Defined in

[hw-ledger/lib/types.ts:13](https://github.com/liquality/chainify/blob/540cfa69/packages/hw-ledger/lib/types.ts#L13)
