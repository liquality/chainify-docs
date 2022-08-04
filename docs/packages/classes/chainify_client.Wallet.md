---
id: "chainify_client.Wallet"
title: "Class: Wallet<T, S>"
sidebar_label: "Wallet"
custom_edit_url: null
---

[@chainify/client](../modules/chainify_client.md).Wallet

## Type parameters

| Name |
| :------ |
| `T` |
| `S` |

## Implements

- `WalletProvider`

## Constructors

### constructor

• **new Wallet**<`T`, `S`\>(`chainProvider?`, `namingProvider?`)

#### Type parameters

| Name |
| :------ |
| `T` |
| `S` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider?` | [`Chain`](chainify_client.Chain.md)<`T`, `Network`\> |
| `namingProvider?` | `NamingProvider` |

#### Defined in

[client/lib/Wallet.ts:20](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L20)

## Properties

### chainProvider

• `Protected` **chainProvider**: [`Chain`](chainify_client.Chain.md)<`T`, `Network`\>

#### Defined in

[client/lib/Wallet.ts:17](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L17)

___

### namingProvider

• `Protected` **namingProvider**: `NamingProvider`

#### Defined in

[client/lib/Wallet.ts:18](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L18)

## Methods

### canUpdateFee

▸ `Abstract` **canUpdateFee**(): `boolean`

#### Returns

`boolean`

#### Implementation of

WalletProvider.canUpdateFee

#### Defined in

[client/lib/Wallet.ts:74](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L74)

___

### exportPrivateKey

▸ `Abstract` **exportPrivateKey**(): `Promise`<`string`\>

#### Returns

`Promise`<`string`\>

#### Implementation of

WalletProvider.exportPrivateKey

#### Defined in

[client/lib/Wallet.ts:70](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L70)

___

### getAddress

▸ `Abstract` **getAddress**(): `Promise`<`AddressType`\>

#### Returns

`Promise`<`AddressType`\>

#### Defined in

[client/lib/Wallet.ts:50](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L50)

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

#### Implementation of

WalletProvider.getAddresses

#### Defined in

[client/lib/Wallet.ts:56](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L56)

___

### getBalance

▸ `Abstract` **getBalance**(`assets`): `Promise`<`BigNumber`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `assets` | `Asset`[] |

#### Returns

`Promise`<`BigNumber`[]\>

#### Defined in

[client/lib/Wallet.ts:68](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L68)

___

### getChainProvider

▸ **getChainProvider**(): [`Chain`](chainify_client.Chain.md)<`T`, `Network`\>

#### Returns

[`Chain`](chainify_client.Chain.md)<`T`, `Network`\>

#### Defined in

[client/lib/Wallet.ts:30](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L30)

___

### getConnectedNetwork

▸ `Abstract` **getConnectedNetwork**(): `Promise`<`Network`\>

#### Returns

`Promise`<`Network`\>

#### Implementation of

WalletProvider.getConnectedNetwork

#### Defined in

[client/lib/Wallet.ts:46](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L46)

___

### getNamingProvider

▸ **getNamingProvider**(): `NamingProvider`

#### Returns

`NamingProvider`

#### Defined in

[client/lib/Wallet.ts:38](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L38)

___

### getSigner

▸ `Abstract` **getSigner**(): `S`

#### Returns

`S`

#### Defined in

[client/lib/Wallet.ts:48](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L48)

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

#### Implementation of

WalletProvider.getUnusedAddress

#### Defined in

[client/lib/Wallet.ts:52](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L52)

___

### getUsedAddresses

▸ `Abstract` **getUsedAddresses**(`numAddressPerCall?`): `Promise`<`Address`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `numAddressPerCall?` | `number` |

#### Returns

`Promise`<`Address`[]\>

#### Implementation of

WalletProvider.getUsedAddresses

#### Defined in

[client/lib/Wallet.ts:54](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L54)

___

### isWalletAvailable

▸ `Abstract` **isWalletAvailable**(): `Promise`<`boolean`\>

#### Returns

`Promise`<`boolean`\>

#### Implementation of

WalletProvider.isWalletAvailable

#### Defined in

[client/lib/Wallet.ts:72](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L72)

___

### onChainProviderUpdate

▸ `Protected` `Abstract` **onChainProviderUpdate**(`chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider` | [`Chain`](chainify_client.Chain.md)<`T`, `Network`\> |

#### Returns

`void`

#### Defined in

[client/lib/Wallet.ts:76](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L76)

___

### sendBatchTransaction

▸ `Abstract` **sendBatchTransaction**(`txRequests`): `Promise`<`Transaction`<`any`\>[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txRequests` | `TransactionRequest`[] |

#### Returns

`Promise`<`Transaction`<`any`\>[]\>

#### Implementation of

WalletProvider.sendBatchTransaction

#### Defined in

[client/lib/Wallet.ts:62](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L62)

___

### sendSweepTransaction

▸ `Abstract` **sendSweepTransaction**(`address`, `asset`, `fee?`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `AddressType` |
| `asset` | `Asset` |
| `fee?` | `FeeType` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Implementation of

WalletProvider.sendSweepTransaction

#### Defined in

[client/lib/Wallet.ts:64](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L64)

___

### sendTransaction

▸ `Abstract` **sendTransaction**(`txRequest`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txRequest` | `TransactionRequest` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Implementation of

WalletProvider.sendTransaction

#### Defined in

[client/lib/Wallet.ts:60](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L60)

___

### setChainProvider

▸ **setChainProvider**(`chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider` | [`Chain`](chainify_client.Chain.md)<`T`, `Network`\> |

#### Returns

`void`

#### Defined in

[client/lib/Wallet.ts:25](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L25)

___

### setNamingProvider

▸ **setNamingProvider**(`namingProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `namingProvider` | `NamingProvider` |

#### Returns

`void`

#### Defined in

[client/lib/Wallet.ts:34](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L34)

___

### signMessage

▸ `Abstract` **signMessage**(`message`, `from`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `from` | `AddressType` |

#### Returns

`Promise`<`string`\>

#### Implementation of

WalletProvider.signMessage

#### Defined in

[client/lib/Wallet.ts:58](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L58)

___

### signTypedData

▸ **signTypedData**(`_data`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_data` | `any` |

#### Returns

`Promise`<`string`\>

#### Defined in

[client/lib/Wallet.ts:42](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L42)

___

### updateTransactionFee

▸ `Abstract` **updateTransactionFee**(`tx`, `newFee`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `tx` | `string` \| `Transaction`<`any`\> |
| `newFee` | `FeeType` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Implementation of

WalletProvider.updateTransactionFee

#### Defined in

[client/lib/Wallet.ts:66](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Wallet.ts#L66)
