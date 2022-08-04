---
id: "chainify_evm.EvmBaseWalletProvider"
title: "Class: EvmBaseWalletProvider<Provider, S>"
sidebar_label: "EvmBaseWalletProvider"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).EvmBaseWalletProvider

## Type parameters

| Name | Type |
| :------ | :------ |
| `Provider` | extends `BaseProvider` |
| `S` | extends `Signer` = `Signer` |

## Hierarchy

- `default`<`Provider`, `S`\>

  ↳ **`EvmBaseWalletProvider`**

  ↳↳ [`EvmWalletProvider`](chainify_evm.EvmWalletProvider.md)

## Constructors

### constructor

• **new EvmBaseWalletProvider**<`Provider`, `S`\>(`chainProvider?`, `namingProvider?`)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `Provider` | extends `BaseProvider`<`Provider`\> |
| `S` | extends `Signer`<`S`\> = `Signer` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider?` | `default`<`Provider`, `Network`\> |
| `namingProvider?` | `NamingProvider` |

#### Overrides

Wallet&lt;Provider, S\&gt;.constructor

#### Defined in

[evm/lib/wallet/EvmBaseWalletProvider.ts:14](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L14)

## Properties

### chainProvider

• `Protected` **chainProvider**: `default`<`Provider`, `Network`\>

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

___

### signer

• `Protected` **signer**: `S`

#### Defined in

[evm/lib/wallet/EvmBaseWalletProvider.ts:12](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L12)

## Methods

### canUpdateFee

▸ `Abstract` **canUpdateFee**(): `boolean`

#### Returns

`boolean`

#### Inherited from

Wallet.canUpdateFee

#### Defined in

client/dist/lib/Wallet.d.ts:26

___

### estimateGas

▸ **estimateGas**(`txRequest`): `Promise`<`BigNumber`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txRequest` | `TransactionRequest` |

#### Returns

`Promise`<`BigNumber`\>

#### Defined in

[evm/lib/wallet/EvmBaseWalletProvider.ts:129](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L129)

___

### exportPrivateKey

▸ `Abstract` **exportPrivateKey**(): `Promise`<`string`\>

#### Returns

`Promise`<`string`\>

#### Inherited from

Wallet.exportPrivateKey

#### Defined in

client/dist/lib/Wallet.d.ts:24

___

### getAddress

▸ `Abstract` **getAddress**(): `Promise`<`AddressType`\>

#### Returns

`Promise`<`AddressType`\>

#### Inherited from

Wallet.getAddress

#### Defined in

client/dist/lib/Wallet.d.ts:14

___

### getAddresses

▸ `Abstract` **getAddresses**(`start?`, `numAddresses?`, `change?`): `Promise`<`Address`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `start?` | `number` |
| `numAddresses?` | `number` |
| `change?` | `boolean` |

#### Returns

`Promise`<`Address`[]\>

#### Inherited from

Wallet.getAddresses

#### Defined in

client/dist/lib/Wallet.d.ts:17

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

[evm/lib/wallet/EvmBaseWalletProvider.ts:120](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L120)

___

### getChainProvider

▸ **getChainProvider**(): `default`<`Provider`, `Network`\>

#### Returns

`default`<`Provider`, `Network`\>

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

[evm/lib/wallet/EvmBaseWalletProvider.ts:125](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L125)

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

▸ **getSigner**(): `S`

#### Returns

`S`

#### Overrides

Wallet.getSigner

#### Defined in

[evm/lib/wallet/EvmBaseWalletProvider.ts:18](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L18)

___

### getUnusedAddress

▸ `Abstract` **getUnusedAddress**(`change?`, `numAddressPerCall?`): `Promise`<`Address`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `change?` | `boolean` |
| `numAddressPerCall?` | `number` |

#### Returns

`Promise`<`Address`\>

#### Inherited from

Wallet.getUnusedAddress

#### Defined in

client/dist/lib/Wallet.d.ts:15

___

### getUsedAddresses

▸ `Abstract` **getUsedAddresses**(`numAddressPerCall?`): `Promise`<`Address`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `numAddressPerCall?` | `number` |

#### Returns

`Promise`<`Address`[]\>

#### Inherited from

Wallet.getUsedAddresses

#### Defined in

client/dist/lib/Wallet.d.ts:16

___

### isWalletAvailable

▸ `Abstract` **isWalletAvailable**(): `Promise`<`boolean`\>

#### Returns

`Promise`<`boolean`\>

#### Inherited from

Wallet.isWalletAvailable

#### Defined in

client/dist/lib/Wallet.d.ts:25

___

### onChainProviderUpdate

▸ `Protected` `Abstract` **onChainProviderUpdate**(`chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider` | `default`<`Provider`, `Network`\> |

#### Returns

`void`

#### Inherited from

Wallet.onChainProviderUpdate

#### Defined in

client/dist/lib/Wallet.d.ts:27

___

### sendBatchTransaction

▸ **sendBatchTransaction**(`txRequests`): `Promise`<`Transaction`<`TransactionResponse`\>[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txRequests` | [`EthereumTransactionRequest`](../namespaces/chainify_evm.EvmTypes.md#ethereumtransactionrequest)[] |

#### Returns

`Promise`<`Transaction`<`TransactionResponse`\>[]\>

#### Overrides

Wallet.sendBatchTransaction

#### Defined in

[evm/lib/wallet/EvmBaseWalletProvider.ts:65](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L65)

___

### sendSweepTransaction

▸ **sendSweepTransaction**(`address`, `asset`, `fee?`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `AddressType` |
| `asset` | `Asset` |
| `fee?` | `FeeType` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Overrides

Wallet.sendSweepTransaction

#### Defined in

[evm/lib/wallet/EvmBaseWalletProvider.ts:74](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L74)

___

### sendTransaction

▸ **sendTransaction**(`txRequest`): `Promise`<`Transaction`<`TransactionResponse`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txRequest` | [`EthereumTransactionRequest`](../namespaces/chainify_evm.EvmTypes.md#ethereumtransactionrequest) |

#### Returns

`Promise`<`Transaction`<`TransactionResponse`\>\>

#### Overrides

Wallet.sendTransaction

#### Defined in

[evm/lib/wallet/EvmBaseWalletProvider.ts:31](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L31)

___

### setChainProvider

▸ **setChainProvider**(`chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider` | `default`<`Provider`, `Network`\> |

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

### setSigner

▸ **setSigner**(`signer`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `signer` | `S` |

#### Returns

`void`

#### Defined in

[evm/lib/wallet/EvmBaseWalletProvider.ts:22](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L22)

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

[evm/lib/wallet/EvmBaseWalletProvider.ts:26](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L26)

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

▸ **updateTransactionFee**(`tx`, `newFee`): `Promise`<`Transaction`<`TransactionResponse`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `tx` | `string` \| `Transaction`<`TransactionResponse`\> |
| `newFee` | `FeeType` |

#### Returns

`Promise`<`Transaction`<`TransactionResponse`\>\>

#### Overrides

Wallet.updateTransactionFee

#### Defined in

[evm/lib/wallet/EvmBaseWalletProvider.ts:80](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L80)
