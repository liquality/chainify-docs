---
id: "chainify_near.NearWalletProvider"
title: "Class: NearWalletProvider"
sidebar_label: "NearWalletProvider"
custom_edit_url: null
---

[@chainify/near](../modules/chainify_near.md).NearWalletProvider

## Hierarchy

- `default`<`providers.JsonRpcProvider`, `InMemorySigner`\>

  ↳ **`NearWalletProvider`**

## Constructors

### constructor

• **new NearWalletProvider**(`walletOptions`, `chainProvider?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `walletOptions` | [`NearWalletOptions`](../interfaces/chainify_near.NearTypes.NearWalletOptions.md) |
| `chainProvider?` | `default`<`JsonRpcProvider`, `Network`\> |

#### Overrides

Wallet&lt;providers.JsonRpcProvider, InMemorySigner\&gt;.constructor

#### Defined in

[near/lib/wallet/NearWalletProvider.ts:28](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/wallet/NearWalletProvider.ts#L28)

## Properties

### chainProvider

• `Protected` **chainProvider**: `default`<`JsonRpcProvider`, `Network`\>

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

[near/lib/wallet/NearWalletProvider.ts:133](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/wallet/NearWalletProvider.ts#L133)

___

### exportPrivateKey

▸ **exportPrivateKey**(): `Promise`<`string`\>

#### Returns

`Promise`<`string`\>

#### Overrides

Wallet.exportPrivateKey

#### Defined in

[near/lib/wallet/NearWalletProvider.ts:125](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/wallet/NearWalletProvider.ts#L125)

___

### getAddress

▸ **getAddress**(): `Promise`<`Address`\>

#### Returns

`Promise`<`Address`\>

#### Overrides

Wallet.getAddress

#### Defined in

[near/lib/wallet/NearWalletProvider.ts:41](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/wallet/NearWalletProvider.ts#L41)

___

### getAddresses

▸ **getAddresses**(): `Promise`<`Address`[]\>

#### Returns

`Promise`<`Address`[]\>

#### Overrides

Wallet.getAddresses

#### Defined in

[near/lib/wallet/NearWalletProvider.ts:72](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/wallet/NearWalletProvider.ts#L72)

___

### getBalance

▸ **getBalance**(`_assets`): `Promise`<`BigNumber`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_assets` | `Asset`[] |

#### Returns

`Promise`<`BigNumber`[]\>

#### Overrides

Wallet.getBalance

#### Defined in

[near/lib/wallet/NearWalletProvider.ts:120](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/wallet/NearWalletProvider.ts#L120)

___

### getChainProvider

▸ **getChainProvider**(): `default`<`JsonRpcProvider`, `Network`\>

#### Returns

`default`<`JsonRpcProvider`, `Network`\>

#### Inherited from

Wallet.getChainProvider

#### Defined in

client/dist/lib/Wallet.d.ts:8

___

### getConnectedNetwork

▸ **getConnectedNetwork**(): `Promise`<[`NearNetwork`](../interfaces/chainify_near.NearTypes.NearNetwork.md)\>

#### Returns

`Promise`<[`NearNetwork`](../interfaces/chainify_near.NearTypes.NearNetwork.md)\>

#### Overrides

Wallet.getConnectedNetwork

#### Defined in

[near/lib/wallet/NearWalletProvider.ts:141](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/wallet/NearWalletProvider.ts#L141)

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

▸ **getSigner**(): `InMemorySigner`

#### Returns

`InMemorySigner`

#### Overrides

Wallet.getSigner

#### Defined in

[near/lib/wallet/NearWalletProvider.ts:37](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/wallet/NearWalletProvider.ts#L37)

___

### getUnusedAddress

▸ **getUnusedAddress**(): `Promise`<`Address`\>

#### Returns

`Promise`<`Address`\>

#### Overrides

Wallet.getUnusedAddress

#### Defined in

[near/lib/wallet/NearWalletProvider.ts:64](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/wallet/NearWalletProvider.ts#L64)

___

### getUsedAddresses

▸ **getUsedAddresses**(): `Promise`<`Address`[]\>

#### Returns

`Promise`<`Address`[]\>

#### Overrides

Wallet.getUsedAddresses

#### Defined in

[near/lib/wallet/NearWalletProvider.ts:68](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/wallet/NearWalletProvider.ts#L68)

___

### isWalletAvailable

▸ **isWalletAvailable**(): `Promise`<`boolean`\>

#### Returns

`Promise`<`boolean`\>

#### Overrides

Wallet.isWalletAvailable

#### Defined in

[near/lib/wallet/NearWalletProvider.ts:129](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/wallet/NearWalletProvider.ts#L129)

___

### onChainProviderUpdate

▸ `Protected` **onChainProviderUpdate**(`_chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `_chainProvider` | `default`<`JsonRpcProvider`, [`NearNetwork`](../interfaces/chainify_near.NearTypes.NearNetwork.md)\> |

#### Returns

`void`

#### Overrides

Wallet.onChainProviderUpdate

#### Defined in

[near/lib/wallet/NearWalletProvider.ts:156](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/wallet/NearWalletProvider.ts#L156)

___

### sendBatchTransaction

▸ **sendBatchTransaction**(`txRequests`): `Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txRequests` | [`NearTxRequest`](../interfaces/chainify_near.NearTypes.NearTxRequest.md)[] |

#### Returns

`Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>[]\>

#### Overrides

Wallet.sendBatchTransaction

#### Defined in

[near/lib/wallet/NearWalletProvider.ts:104](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/wallet/NearWalletProvider.ts#L104)

___

### sendSweepTransaction

▸ **sendSweepTransaction**(`to`, `_asset`): `Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `to` | `AddressType` |
| `_asset` | `Asset` |

#### Returns

`Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Overrides

Wallet.sendSweepTransaction

#### Defined in

[near/lib/wallet/NearWalletProvider.ts:113](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/wallet/NearWalletProvider.ts#L113)

___

### sendTransaction

▸ **sendTransaction**(`txRequest`): `Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txRequest` | [`NearTxRequest`](../interfaces/chainify_near.NearTypes.NearTxRequest.md) |

#### Returns

`Promise`<`Transaction`<[`NearTxLog`](../interfaces/chainify_near.NearTypes.NearTxLog.md)\>\>

#### Overrides

Wallet.sendTransaction

#### Defined in

[near/lib/wallet/NearWalletProvider.ts:89](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/wallet/NearWalletProvider.ts#L89)

___

### setChainProvider

▸ **setChainProvider**(`chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider` | `default`<`JsonRpcProvider`, `Network`\> |

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

▸ **signMessage**(`message`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |

#### Returns

`Promise`<`string`\>

#### Overrides

Wallet.signMessage

#### Defined in

[near/lib/wallet/NearWalletProvider.ts:77](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/wallet/NearWalletProvider.ts#L77)

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

▸ **updateTransactionFee**(`_tx`): `Promise`<`Transaction`<[`NearTxResponse`](../interfaces/chainify_near.NearTypes.NearTxResponse.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_tx` | `string` \| `Transaction`<`any`\> |

#### Returns

`Promise`<`Transaction`<[`NearTxResponse`](../interfaces/chainify_near.NearTypes.NearTxResponse.md)\>\>

#### Overrides

Wallet.updateTransactionFee

#### Defined in

[near/lib/wallet/NearWalletProvider.ts:137](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/wallet/NearWalletProvider.ts#L137)
