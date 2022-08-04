---
id: "chainify_evm.EvmWalletProvider"
title: "Class: EvmWalletProvider"
sidebar_label: "EvmWalletProvider"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).EvmWalletProvider

## Hierarchy

- [`EvmBaseWalletProvider`](chainify_evm.EvmBaseWalletProvider.md)<`StaticJsonRpcProvider`, `EthersWallet`\>

  ↳ **`EvmWalletProvider`**

## Constructors

### constructor

• **new EvmWalletProvider**(`walletOptions`, `chainProvider?`, `namingProvider?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `walletOptions` | `WalletOptions` |
| `chainProvider?` | `default`<`StaticJsonRpcProvider`, `Network`\> |
| `namingProvider?` | `NamingProvider` |

#### Overrides

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[constructor](chainify_evm.EvmBaseWalletProvider.md#constructor)

#### Defined in

[evm/lib/wallet/EvmWalletProvider.ts:14](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmWalletProvider.ts#L14)

## Properties

### chainProvider

• `Protected` **chainProvider**: `default`<`StaticJsonRpcProvider`, `Network`\>

#### Inherited from

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[chainProvider](chainify_evm.EvmBaseWalletProvider.md#chainprovider)

#### Defined in

client/dist/lib/Wallet.d.ts:4

___

### namingProvider

• `Protected` **namingProvider**: `NamingProvider`

#### Inherited from

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[namingProvider](chainify_evm.EvmBaseWalletProvider.md#namingprovider)

#### Defined in

client/dist/lib/Wallet.d.ts:5

___

### signer

• `Protected` **signer**: `Wallet`

#### Inherited from

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[signer](chainify_evm.EvmBaseWalletProvider.md#signer)

#### Defined in

[evm/lib/wallet/EvmBaseWalletProvider.ts:12](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L12)

## Methods

### canUpdateFee

▸ **canUpdateFee**(): `boolean`

#### Returns

`boolean`

#### Overrides

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[canUpdateFee](chainify_evm.EvmBaseWalletProvider.md#canupdatefee)

#### Defined in

[evm/lib/wallet/EvmWalletProvider.ts:78](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmWalletProvider.ts#L78)

___

### estimateGas

▸ **estimateGas**(`txRequest`): `Promise`<`BigNumber`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txRequest` | `TransactionRequest` |

#### Returns

`Promise`<`BigNumber`\>

#### Inherited from

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[estimateGas](chainify_evm.EvmBaseWalletProvider.md#estimategas)

#### Defined in

[evm/lib/wallet/EvmBaseWalletProvider.ts:129](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L129)

___

### exportPrivateKey

▸ **exportPrivateKey**(): `Promise`<`string`\>

#### Returns

`Promise`<`string`\>

#### Overrides

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[exportPrivateKey](chainify_evm.EvmBaseWalletProvider.md#exportprivatekey)

#### Defined in

[evm/lib/wallet/EvmWalletProvider.ts:70](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmWalletProvider.ts#L70)

___

### getAddress

▸ **getAddress**(): `Promise`<`Address`\>

#### Returns

`Promise`<`Address`\>

#### Overrides

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[getAddress](chainify_evm.EvmBaseWalletProvider.md#getaddress)

#### Defined in

[evm/lib/wallet/EvmWalletProvider.ts:26](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmWalletProvider.ts#L26)

___

### getAddresses

▸ **getAddresses**(): `Promise`<`Address`[]\>

#### Returns

`Promise`<`Address`[]\>

#### Overrides

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[getAddresses](chainify_evm.EvmBaseWalletProvider.md#getaddresses)

#### Defined in

[evm/lib/wallet/EvmWalletProvider.ts:65](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmWalletProvider.ts#L65)

___

### getBalance

▸ **getBalance**(`assets`): `Promise`<`BigNumber`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `assets` | `Asset`[] |

#### Returns

`Promise`<`BigNumber`[]\>

#### Inherited from

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[getBalance](chainify_evm.EvmBaseWalletProvider.md#getbalance)

#### Defined in

[evm/lib/wallet/EvmBaseWalletProvider.ts:120](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L120)

___

### getChainProvider

▸ **getChainProvider**(): `default`<`StaticJsonRpcProvider`, `Network`\>

#### Returns

`default`<`StaticJsonRpcProvider`, `Network`\>

#### Inherited from

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[getChainProvider](chainify_evm.EvmBaseWalletProvider.md#getchainprovider)

#### Defined in

client/dist/lib/Wallet.d.ts:8

___

### getConnectedNetwork

▸ **getConnectedNetwork**(): `Promise`<`Network`\>

#### Returns

`Promise`<`Network`\>

#### Inherited from

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[getConnectedNetwork](chainify_evm.EvmBaseWalletProvider.md#getconnectednetwork)

#### Defined in

[evm/lib/wallet/EvmBaseWalletProvider.ts:125](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L125)

___

### getNamingProvider

▸ **getNamingProvider**(): `NamingProvider`

#### Returns

`NamingProvider`

#### Inherited from

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[getNamingProvider](chainify_evm.EvmBaseWalletProvider.md#getnamingprovider)

#### Defined in

client/dist/lib/Wallet.d.ts:10

___

### getSigner

▸ **getSigner**(): `Wallet`

#### Returns

`Wallet`

#### Inherited from

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[getSigner](chainify_evm.EvmBaseWalletProvider.md#getsigner)

#### Defined in

[evm/lib/wallet/EvmBaseWalletProvider.ts:18](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L18)

___

### getUnusedAddress

▸ **getUnusedAddress**(): `Promise`<`Address`\>

#### Returns

`Promise`<`Address`\>

#### Overrides

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[getUnusedAddress](chainify_evm.EvmBaseWalletProvider.md#getunusedaddress)

#### Defined in

[evm/lib/wallet/EvmWalletProvider.ts:57](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmWalletProvider.ts#L57)

___

### getUsedAddresses

▸ **getUsedAddresses**(): `Promise`<`Address`[]\>

#### Returns

`Promise`<`Address`[]\>

#### Overrides

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[getUsedAddresses](chainify_evm.EvmBaseWalletProvider.md#getusedaddresses)

#### Defined in

[evm/lib/wallet/EvmWalletProvider.ts:61](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmWalletProvider.ts#L61)

___

### isWalletAvailable

▸ **isWalletAvailable**(): `Promise`<`boolean`\>

#### Returns

`Promise`<`boolean`\>

#### Overrides

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[isWalletAvailable](chainify_evm.EvmBaseWalletProvider.md#iswalletavailable)

#### Defined in

[evm/lib/wallet/EvmWalletProvider.ts:74](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmWalletProvider.ts#L74)

___

### onChainProviderUpdate

▸ `Protected` **onChainProviderUpdate**(`chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider` | `default`<`StaticJsonRpcProvider`, `Network`\> |

#### Returns

`void`

#### Overrides

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[onChainProviderUpdate](chainify_evm.EvmBaseWalletProvider.md#onchainproviderupdate)

#### Defined in

[evm/lib/wallet/EvmWalletProvider.ts:82](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmWalletProvider.ts#L82)

___

### sendBatchTransaction

▸ **sendBatchTransaction**(`txRequests`): `Promise`<`Transaction`<`TransactionResponse`\>[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txRequests` | [`EthereumTransactionRequest`](../namespaces/chainify_evm.EvmTypes.md#ethereumtransactionrequest)[] |

#### Returns

`Promise`<`Transaction`<`TransactionResponse`\>[]\>

#### Inherited from

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[sendBatchTransaction](chainify_evm.EvmBaseWalletProvider.md#sendbatchtransaction)

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

#### Inherited from

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[sendSweepTransaction](chainify_evm.EvmBaseWalletProvider.md#sendsweeptransaction)

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

#### Inherited from

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[sendTransaction](chainify_evm.EvmBaseWalletProvider.md#sendtransaction)

#### Defined in

[evm/lib/wallet/EvmBaseWalletProvider.ts:31](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L31)

___

### setChainProvider

▸ **setChainProvider**(`chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider` | `default`<`StaticJsonRpcProvider`, `Network`\> |

#### Returns

`void`

#### Inherited from

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[setChainProvider](chainify_evm.EvmBaseWalletProvider.md#setchainprovider)

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

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[setNamingProvider](chainify_evm.EvmBaseWalletProvider.md#setnamingprovider)

#### Defined in

client/dist/lib/Wallet.d.ts:9

___

### setSigner

▸ **setSigner**(`signer`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `signer` | `Wallet` |

#### Returns

`void`

#### Inherited from

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[setSigner](chainify_evm.EvmBaseWalletProvider.md#setsigner)

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

#### Inherited from

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[signMessage](chainify_evm.EvmBaseWalletProvider.md#signmessage)

#### Defined in

[evm/lib/wallet/EvmBaseWalletProvider.ts:26](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L26)

___

### signTypedData

▸ **signTypedData**(`__namedParameters`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters` | [`SignTypedMessageType`](../interfaces/chainify_evm.EvmTypes.SignTypedMessageType.md)<`SignTypedDataVersion`, `MessageTypes`\> |

#### Returns

`Promise`<`string`\>

#### Overrides

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[signTypedData](chainify_evm.EvmBaseWalletProvider.md#signtypeddata)

#### Defined in

[evm/lib/wallet/EvmWalletProvider.ts:37](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmWalletProvider.ts#L37)

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

#### Inherited from

[EvmBaseWalletProvider](chainify_evm.EvmBaseWalletProvider.md).[updateTransactionFee](chainify_evm.EvmBaseWalletProvider.md#updatetransactionfee)

#### Defined in

[evm/lib/wallet/EvmBaseWalletProvider.ts:80](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/wallet/EvmBaseWalletProvider.ts#L80)
