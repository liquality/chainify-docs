---
id: "chainify_hw_ledger.LedgerProvider"
title: "Class: LedgerProvider<TApp>"
sidebar_label: "LedgerProvider"
custom_edit_url: null
---

[@chainify/hw-ledger](../modules/chainify_hw_ledger.md).LedgerProvider

## Type parameters

| Name | Type |
| :------ | :------ |
| `TApp` | extends [`HWApp`](../namespaces/chainify_hw_ledger.LedgerProviderTypes.md#hwapp) |

## Constructors

### constructor

• **new LedgerProvider**<`TApp`\>(`appType`, `options`)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `TApp` | extends [`HWApp`](../namespaces/chainify_hw_ledger.LedgerProviderTypes.md#hwapp) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `appType` | [`Newable`](../namespaces/chainify_hw_ledger.LedgerProviderTypes.md#newable)<`TApp`\> |
| `options` | [`CreateOptions`](../interfaces/chainify_hw_ledger.LedgerProviderTypes.CreateOptions.md) |

#### Defined in

[hw-ledger/lib/LedgerProvider.ts:20](https://github.com/liquality/chainify/blob/540cfa69/packages/hw-ledger/lib/LedgerProvider.ts#L20)

## Properties

### \_appInstance

• `Protected` **\_appInstance**: `TApp`

#### Defined in

[hw-ledger/lib/LedgerProvider.ts:18](https://github.com/liquality/chainify/blob/540cfa69/packages/hw-ledger/lib/LedgerProvider.ts#L18)

___

### \_transport

• `Protected` **\_transport**: `default`

#### Defined in

[hw-ledger/lib/LedgerProvider.ts:17](https://github.com/liquality/chainify/blob/540cfa69/packages/hw-ledger/lib/LedgerProvider.ts#L17)

## Methods

### errorProxy

▸ `Protected` **errorProxy**(`target`, `func`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `target` | `any` |
| `func` | `string` |

#### Returns

`any`

#### Defined in

[hw-ledger/lib/LedgerProvider.ts:95](https://github.com/liquality/chainify/blob/540cfa69/packages/hw-ledger/lib/LedgerProvider.ts#L95)

___

### getApp

▸ **getApp**(): `Promise`<`TApp`\>

#### Returns

`Promise`<`TApp`\>

#### Defined in

[hw-ledger/lib/LedgerProvider.ts:81](https://github.com/liquality/chainify/blob/540cfa69/packages/hw-ledger/lib/LedgerProvider.ts#L81)

___

### getConnectedNetwork

▸ **getConnectedNetwork**(): `Promise`<`Network`\>

#### Returns

`Promise`<`Network`\>

#### Defined in

[hw-ledger/lib/LedgerProvider.ts:50](https://github.com/liquality/chainify/blob/540cfa69/packages/hw-ledger/lib/LedgerProvider.ts#L50)

___

### getWalletAddress

▸ **getWalletAddress**(`address`, `getAddresses`): `Promise`<`Address`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `getAddresses` | [`GetAddressesFuncType`](../namespaces/chainify_hw_ledger.LedgerProviderTypes.md#getaddressesfunctype) |

#### Returns

`Promise`<`Address`\>

#### Defined in

[hw-ledger/lib/LedgerProvider.ts:55](https://github.com/liquality/chainify/blob/540cfa69/packages/hw-ledger/lib/LedgerProvider.ts#L55)

___

### isWalletAvailable

▸ **isWalletAvailable**(): `Promise`<`boolean`\>

#### Returns

`Promise`<`boolean`\>

#### Defined in

[hw-ledger/lib/LedgerProvider.ts:30](https://github.com/liquality/chainify/blob/540cfa69/packages/hw-ledger/lib/LedgerProvider.ts#L30)
