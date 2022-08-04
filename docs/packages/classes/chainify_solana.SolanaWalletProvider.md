---
id: "chainify_solana.SolanaWalletProvider"
title: "Class: SolanaWalletProvider"
sidebar_label: "SolanaWalletProvider"
custom_edit_url: null
---

[@chainify/solana](../modules/chainify_solana.md).SolanaWalletProvider

## Hierarchy

- `default`<`Connection`, `Promise`<`Keypair`\>\>

  ↳ **`SolanaWalletProvider`**

## Constructors

### constructor

• **new SolanaWalletProvider**(`walletOptions`, `chainProvider?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `walletOptions` | `WalletOptions` |
| `chainProvider?` | [`SolanaChainProvider`](chainify_solana.SolanaChainProvider.md) |

#### Overrides

Wallet&lt;Connection, Promise&lt;Keypair\&gt;\&gt;.constructor

#### Defined in

[solana/lib/wallet/SolanaWalletProvider.ts:32](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/wallet/SolanaWalletProvider.ts#L32)

## Properties

### chainProvider

• `Protected` **chainProvider**: `default`<`Connection`, `Network`\>

#### Inherited from

Wallet.chainProvider

#### Defined in

client/dist/lib/Wallet.d.ts:4

___

### namingProvider

• `Protected` **namingProvider**: `NamingProvider`

#### Inherited from

Wallet.namingProvider

#### Defined in

client/dist/lib/Wallet.d.ts:5

## Methods

### canUpdateFee

▸ **canUpdateFee**(): `boolean`

#### Returns

`boolean`

#### Overrides

Wallet.canUpdateFee

#### Defined in

[solana/lib/wallet/SolanaWalletProvider.ts:163](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/wallet/SolanaWalletProvider.ts#L163)

___

### exportPrivateKey

▸ **exportPrivateKey**(): `Promise`<`string`\>

#### Returns

`Promise`<`string`\>

#### Overrides

Wallet.exportPrivateKey

#### Defined in

[solana/lib/wallet/SolanaWalletProvider.ts:154](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/wallet/SolanaWalletProvider.ts#L154)

___

### getAddress

▸ **getAddress**(): `Promise`<`Address`\>

#### Returns

`Promise`<`Address`\>

#### Overrides

Wallet.getAddress

#### Defined in

[solana/lib/wallet/SolanaWalletProvider.ts:50](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/wallet/SolanaWalletProvider.ts#L50)

___

### getAddresses

▸ **getAddresses**(): `Promise`<`Address`[]\>

#### Returns

`Promise`<`Address`[]\>

#### Overrides

Wallet.getAddresses

#### Defined in

[solana/lib/wallet/SolanaWalletProvider.ts:74](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/wallet/SolanaWalletProvider.ts#L74)

___

### getBalance

▸ **getBalance**(`assets`): `Promise`<`BigNumber`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `assets` | `Asset`[] |

#### Returns

`Promise`<`BigNumber`[]\>

#### Overrides

Wallet.getBalance

#### Defined in

[solana/lib/wallet/SolanaWalletProvider.ts:149](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/wallet/SolanaWalletProvider.ts#L149)

___

### getChainProvider

▸ **getChainProvider**(): `default`<`Connection`, `Network`\>

#### Returns

`default`<`Connection`, `Network`\>

#### Inherited from

Wallet.getChainProvider

#### Defined in

client/dist/lib/Wallet.d.ts:8

___

### getConnectedNetwork

▸ **getConnectedNetwork**(): `Promise`<`Network`\>

#### Returns

`Promise`<`Network`\>

#### Overrides

Wallet.getConnectedNetwork

#### Defined in

[solana/lib/wallet/SolanaWalletProvider.ts:42](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/wallet/SolanaWalletProvider.ts#L42)

___

### getNamingProvider

▸ **getNamingProvider**(): `NamingProvider`

#### Returns

`NamingProvider`

#### Inherited from

Wallet.getNamingProvider

#### Defined in

client/dist/lib/Wallet.d.ts:10

___

### getSigner

▸ **getSigner**(): `Promise`<`Keypair`\>

#### Returns

`Promise`<`Keypair`\>

#### Overrides

Wallet.getSigner

#### Defined in

[solana/lib/wallet/SolanaWalletProvider.ts:46](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/wallet/SolanaWalletProvider.ts#L46)

___

### getUnusedAddress

▸ **getUnusedAddress**(): `Promise`<`Address`\>

#### Returns

`Promise`<`Address`\>

#### Overrides

Wallet.getUnusedAddress

#### Defined in

[solana/lib/wallet/SolanaWalletProvider.ts:65](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/wallet/SolanaWalletProvider.ts#L65)

___

### getUsedAddresses

▸ **getUsedAddresses**(): `Promise`<`Address`[]\>

#### Returns

`Promise`<`Address`[]\>

#### Overrides

Wallet.getUsedAddresses

#### Defined in

[solana/lib/wallet/SolanaWalletProvider.ts:70](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/wallet/SolanaWalletProvider.ts#L70)

___

### isWalletAvailable

▸ **isWalletAvailable**(): `Promise`<`boolean`\>

#### Returns

`Promise`<`boolean`\>

#### Overrides

Wallet.isWalletAvailable

#### Defined in

[solana/lib/wallet/SolanaWalletProvider.ts:158](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/wallet/SolanaWalletProvider.ts#L158)

___

### onChainProviderUpdate

▸ `Protected` **onChainProviderUpdate**(`_chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `_chainProvider` | [`SolanaChainProvider`](chainify_solana.SolanaChainProvider.md) |

#### Returns

`void`

#### Overrides

Wallet.onChainProviderUpdate

#### Defined in

[solana/lib/wallet/SolanaWalletProvider.ts:167](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/wallet/SolanaWalletProvider.ts#L167)

___

### sendBatchTransaction

▸ **sendBatchTransaction**(`txRequests`): `Promise`<`Transaction`<`any`\>[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txRequests` | `TransactionRequest`[] |

#### Returns

`Promise`<`Transaction`<`any`\>[]\>

#### Overrides

Wallet.sendBatchTransaction

#### Defined in

[solana/lib/wallet/SolanaWalletProvider.ts:130](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/wallet/SolanaWalletProvider.ts#L130)

___

### sendSweepTransaction

▸ **sendSweepTransaction**(`address`, `asset`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `AddressType` |
| `asset` | `Asset` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Overrides

Wallet.sendSweepTransaction

#### Defined in

[solana/lib/wallet/SolanaWalletProvider.ts:139](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/wallet/SolanaWalletProvider.ts#L139)

___

### sendTransaction

▸ **sendTransaction**(`txRequest`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txRequest` | `TransactionRequest` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Overrides

Wallet.sendTransaction

#### Defined in

[solana/lib/wallet/SolanaWalletProvider.ts:86](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/wallet/SolanaWalletProvider.ts#L86)

___

### setChainProvider

▸ **setChainProvider**(`chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider` | `default`<`Connection`, `Network`\> |

#### Returns

`void`

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

#### Inherited from

Wallet.setNamingProvider

#### Defined in

client/dist/lib/Wallet.d.ts:9

___

### signMessage

▸ **signMessage**(`message`, `_from`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `_from` | `AddressType` |

#### Returns

`Promise`<`string`\>

#### Overrides

Wallet.signMessage

#### Defined in

[solana/lib/wallet/SolanaWalletProvider.ts:79](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/wallet/SolanaWalletProvider.ts#L79)

___

### signTypedData

▸ **signTypedData**(`_data`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_data` | `any` |

#### Returns

`Promise`<`string`\>

#### Inherited from

Wallet.signTypedData

#### Defined in

client/dist/lib/Wallet.d.ts:11

___

### updateTransactionFee

▸ **updateTransactionFee**(`_tx`, `_newFee`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_tx` | `string` \| `Transaction`<`any`\> |
| `_newFee` | `FeeType` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Overrides

Wallet.updateTransactionFee

#### Defined in

[solana/lib/wallet/SolanaWalletProvider.ts:145](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/wallet/SolanaWalletProvider.ts#L145)
