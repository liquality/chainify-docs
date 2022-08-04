---
id: "chainify_bitcoin.BitcoinNodeWalletProvider"
title: "Class: BitcoinNodeWalletProvider"
sidebar_label: "BitcoinNodeWalletProvider"
custom_edit_url: null
---

[@chainify/bitcoin](../modules/chainify_bitcoin.md).BitcoinNodeWalletProvider

## Hierarchy

- `default`<`any`, `any`\>

  ↳ **`BitcoinNodeWalletProvider`**

## Implements

- `IBitcoinWallet`<[`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md)\>

## Constructors

### constructor

• **new BitcoinNodeWalletProvider**(`options?`, `chainProvider?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `options?` | [`BitcoinNodeWalletOptions`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinNodeWalletOptions.md) |
| `chainProvider?` | `default`<[`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md), `Network`\> |

#### Overrides

Wallet&lt;any, any\&gt;.constructor

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:30](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L30)

## Properties

### chainProvider

• `Protected` **chainProvider**: `default`<`any`, `Network`\>

#### Implementation of

IBitcoinWallet.chainProvider

#### Inherited from

Wallet.chainProvider

#### Defined in

client/dist/lib/Wallet.d.ts:4

___

### namingProvider

• `Protected` **namingProvider**: `NamingProvider`

#### Implementation of

IBitcoinWallet.namingProvider

#### Inherited from

Wallet.namingProvider

#### Defined in

client/dist/lib/Wallet.d.ts:5

## Methods

### canUpdateFee

▸ **canUpdateFee**(): `boolean`

#### Returns

`boolean`

#### Implementation of

IBitcoinWallet.canUpdateFee

#### Overrides

Wallet.canUpdateFee

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:128](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L128)

___

### exportPrivateKey

▸ **exportPrivateKey**(): `Promise`<`string`\>

#### Returns

`Promise`<`string`\>

#### Implementation of

IBitcoinWallet.exportPrivateKey

#### Overrides

Wallet.exportPrivateKey

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:114](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L114)

___

### getAddress

▸ **getAddress**(): `Promise`<`AddressType`\>

#### Returns

`Promise`<`AddressType`\>

#### Implementation of

IBitcoinWallet.getAddress

#### Overrides

Wallet.getAddress

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:98](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L98)

___

### getAddresses

▸ **getAddresses**(): `Promise`<`Address`[]\>

#### Returns

`Promise`<`Address`[]\>

#### Implementation of

IBitcoinWallet.getAddresses

#### Overrides

Wallet.getAddresses

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:50](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L50)

___

### getBalance

▸ **getBalance**(`assets`): `Promise`<`BigNumber`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `assets` | `Asset`[] |

#### Returns

`Promise`<`BigNumber`[]\>

#### Implementation of

IBitcoinWallet.getBalance

#### Overrides

Wallet.getBalance

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:109](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L109)

___

### getChainProvider

▸ **getChainProvider**(): `default`<`any`, `Network`\>

#### Returns

`default`<`any`, `Network`\>

#### Implementation of

IBitcoinWallet.getChainProvider

#### Inherited from

Wallet.getChainProvider

#### Defined in

client/dist/lib/Wallet.d.ts:8

___

### getConnectedNetwork

▸ **getConnectedNetwork**(): `Promise`<`Network`\>

#### Returns

`Promise`<`Network`\>

#### Implementation of

IBitcoinWallet.getConnectedNetwork

#### Overrides

Wallet.getConnectedNetwork

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:88](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L88)

___

### getNamingProvider

▸ **getNamingProvider**(): `NamingProvider`

#### Returns

`NamingProvider`

#### Implementation of

IBitcoinWallet.getNamingProvider

#### Inherited from

Wallet.getNamingProvider

#### Defined in

client/dist/lib/Wallet.d.ts:10

___

### getSigner

▸ **getSigner**(): `Promise`<``null``\>

#### Returns

`Promise`<``null``\>

#### Implementation of

IBitcoinWallet.getSigner

#### Overrides

Wallet.getSigner

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:94](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L94)

___

### getUnusedAddress

▸ **getUnusedAddress**(): `Promise`<`Address`\>

#### Returns

`Promise`<`Address`\>

#### Implementation of

IBitcoinWallet.getUnusedAddress

#### Overrides

Wallet.getUnusedAddress

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:38](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L38)

___

### getUsedAddresses

▸ **getUsedAddresses**(): `Promise`<`Address`[]\>

#### Returns

`Promise`<`Address`[]\>

#### Implementation of

IBitcoinWallet.getUsedAddresses

#### Overrides

Wallet.getUsedAddresses

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:42](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L42)

___

### getWalletAddress

▸ **getWalletAddress**(`address`): `Promise`<`Address`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |

#### Returns

`Promise`<`Address`\>

#### Implementation of

IBitcoinWallet.getWalletAddress

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:181](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L181)

___

### isWalletAvailable

▸ **isWalletAvailable**(): `Promise`<`boolean`\>

#### Returns

`Promise`<`boolean`\>

#### Implementation of

IBitcoinWallet.isWalletAvailable

#### Overrides

Wallet.isWalletAvailable

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:119](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L119)

___

### onChainProviderUpdate

▸ `Protected` **onChainProviderUpdate**(`chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider` | `default`<[`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md), `Network`\> |

#### Returns

`void`

#### Implementation of

IBitcoinWallet.onChainProviderUpdate

#### Overrides

Wallet.onChainProviderUpdate

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:185](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L185)

___

### sendBatchTransaction

▸ **sendBatchTransaction**(`transactions`): `Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `transactions` | `TransactionRequest`[] |

#### Returns

`Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>[]\>

#### Implementation of

IBitcoinWallet.sendBatchTransaction

#### Overrides

Wallet.sendBatchTransaction

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:60](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L60)

___

### sendSweepTransaction

▸ **sendSweepTransaction**(`_address`, `_asset`, `_fee?`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_address` | `AddressType` |
| `_asset` | `Asset` |
| `_fee?` | `FeeType` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Implementation of

IBitcoinWallet.sendSweepTransaction

#### Overrides

Wallet.sendSweepTransaction

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:74](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L74)

___

### sendTransaction

▸ **sendTransaction**(`txRequest`): `Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txRequest` | `TransactionRequest` |

#### Returns

`Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Implementation of

IBitcoinWallet.sendTransaction

#### Overrides

Wallet.sendTransaction

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:54](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L54)

___

### setChainProvider

▸ **setChainProvider**(`chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider` | `default`<`any`, `Network`\> |

#### Returns

`void`

#### Implementation of

IBitcoinWallet.setChainProvider

#### Inherited from

Wallet.setChainProvider

#### Defined in

client/dist/lib/Wallet.d.ts:7

___

### setNamingProvider

▸ **setNamingProvider**(`namingProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `namingProvider` | `NamingProvider` |

#### Returns

`void`

#### Implementation of

IBitcoinWallet.setNamingProvider

#### Inherited from

Wallet.setNamingProvider

#### Defined in

client/dist/lib/Wallet.d.ts:9

___

### signBatchP2SHTransaction

▸ **signBatchP2SHTransaction**(`inputs`, `addresses`, `tx`, `locktime`, `segwit?`): `Promise`<`Buffer`[]\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `inputs` | [{ `index`: `number` ; `inputTxHex`: `string` ; `outputScript`: `Buffer` ; `vout`: `any`  }] | `undefined` |
| `addresses` | `string` | `undefined` |
| `tx` | `any` | `undefined` |
| `locktime` | `number` | `undefined` |
| `segwit` | `boolean` | `false` |

#### Returns

`Promise`<`Buffer`[]\>

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:146](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L146)

___

### signMessage

▸ **signMessage**(`message`, `from`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `from` | `string` |

#### Returns

`Promise`<`string`\>

#### Implementation of

IBitcoinWallet.signMessage

#### Overrides

Wallet.signMessage

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:103](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L103)

___

### signPSBT

▸ **signPSBT**(`data`, `inputs`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | `string` |
| `inputs` | [`PsbtInputTarget`](../interfaces/chainify_bitcoin.BitcoinTypes.PsbtInputTarget.md)[] |

#### Returns

`Promise`<`string`\>

#### Implementation of

IBitcoinWallet.signPSBT

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:132](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L132)

___

### signTypedData

▸ **signTypedData**(`_data`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_data` | `any` |

#### Returns

`Promise`<`string`\>

#### Implementation of

IBitcoinWallet.signTypedData

#### Inherited from

Wallet.signTypedData

#### Defined in

client/dist/lib/Wallet.d.ts:11

___

### updateTransactionFee

▸ **updateTransactionFee**(`tx`, `newFee`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `tx` | `string` \| `Transaction`<`any`\> |
| `newFee` | `number` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Implementation of

IBitcoinWallet.updateTransactionFee

#### Overrides

Wallet.updateTransactionFee

#### Defined in

[bitcoin/lib/wallet/BitcoinNodeWallet.ts:78](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinNodeWallet.ts#L78)
