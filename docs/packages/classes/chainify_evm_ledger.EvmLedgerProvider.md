---
id: "chainify_evm_ledger.EvmLedgerProvider"
title: "Class: EvmLedgerProvider"
sidebar_label: "EvmLedgerProvider"
custom_edit_url: null
---

[@chainify/evm-ledger](../modules/chainify_evm_ledger.md).EvmLedgerProvider

## Hierarchy

- `EvmBaseWalletProvider`<`StaticJsonRpcProvider`, [`EvmLedgerSigner`](chainify_evm_ledger.EvmLedgerSigner.md)\>

  ↳ **`EvmLedgerProvider`**

## Constructors

### constructor

• **new EvmLedgerProvider**(`options`, `chainProvider?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`EvmLedgerCreateOptions`](../interfaces/chainify_evm_ledger.EvmLedgerProviderTypes.EvmLedgerCreateOptions.md) |
| `chainProvider?` | `default`<`StaticJsonRpcProvider`, `Network`\> |

#### Overrides

EvmBaseWalletProvider&lt;StaticJsonRpcProvider, EvmLedgerSigner\&gt;.constructor

#### Defined in

[evm-ledger/lib/EvmLedgerProvider.ts:20](https://github.com/liquality/chainify/blob/540cfa69/packages/evm-ledger/lib/EvmLedgerProvider.ts#L20)

## Properties

### chainProvider

• `Protected` **chainProvider**: `default`<`StaticJsonRpcProvider`, `Network`\>

#### Inherited from

EvmBaseWalletProvider.chainProvider

#### Defined in

client/dist/lib/Wallet.d.ts:4

___

### namingProvider

• `Protected` **namingProvider**: `NamingProvider`

#### Inherited from

EvmBaseWalletProvider.namingProvider

#### Defined in

client/dist/lib/Wallet.d.ts:5

___

### signer

• `Protected` **signer**: [`EvmLedgerSigner`](chainify_evm_ledger.EvmLedgerSigner.md)

#### Inherited from

EvmBaseWalletProvider.signer

#### Defined in

evm/dist/lib/wallet/EvmBaseWalletProvider.d.ts:7

## Methods

### canUpdateFee

▸ **canUpdateFee**(): `boolean`

#### Returns

`boolean`

#### Overrides

EvmBaseWalletProvider.canUpdateFee

#### Defined in

[evm-ledger/lib/EvmLedgerProvider.ts:104](https://github.com/liquality/chainify/blob/540cfa69/packages/evm-ledger/lib/EvmLedgerProvider.ts#L104)

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

EvmBaseWalletProvider.estimateGas

#### Defined in

evm/dist/lib/wallet/EvmBaseWalletProvider.d.ts:18

___

### exportPrivateKey

▸ **exportPrivateKey**(): `Promise`<`string`\>

#### Returns

`Promise`<`string`\>

#### Overrides

EvmBaseWalletProvider.exportPrivateKey

#### Defined in

[evm-ledger/lib/EvmLedgerProvider.ts:92](https://github.com/liquality/chainify/blob/540cfa69/packages/evm-ledger/lib/EvmLedgerProvider.ts#L92)

___

### getAddress

▸ **getAddress**(): `Promise`<`Address`\>

#### Returns

`Promise`<`Address`\>

#### Overrides

EvmBaseWalletProvider.getAddress

#### Defined in

[evm-ledger/lib/EvmLedgerProvider.ts:57](https://github.com/liquality/chainify/blob/540cfa69/packages/evm-ledger/lib/EvmLedgerProvider.ts#L57)

___

### getAddresses

▸ **getAddresses**(): `Promise`<`Address`[]\>

#### Returns

`Promise`<`Address`[]\>

#### Overrides

EvmBaseWalletProvider.getAddresses

#### Defined in

[evm-ledger/lib/EvmLedgerProvider.ts:70](https://github.com/liquality/chainify/blob/540cfa69/packages/evm-ledger/lib/EvmLedgerProvider.ts#L70)

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

EvmBaseWalletProvider.getBalance

#### Defined in

evm/dist/lib/wallet/EvmBaseWalletProvider.d.ts:16

___

### getChainProvider

▸ **getChainProvider**(): `default`<`StaticJsonRpcProvider`, `Network`\>

#### Returns

`default`<`StaticJsonRpcProvider`, `Network`\>

#### Inherited from

EvmBaseWalletProvider.getChainProvider

#### Defined in

client/dist/lib/Wallet.d.ts:8

___

### getConnectedNetwork

▸ **getConnectedNetwork**(): `Promise`<`Network`\>

#### Returns

`Promise`<`Network`\>

#### Overrides

EvmBaseWalletProvider.getConnectedNetwork

#### Defined in

[evm-ledger/lib/EvmLedgerProvider.ts:100](https://github.com/liquality/chainify/blob/540cfa69/packages/evm-ledger/lib/EvmLedgerProvider.ts#L100)

___

### getLedgerAddress

▸ **getLedgerAddress**(): `Promise`<{ `address`: `string` ; `chainCode?`: `string` ; `publicKey`: `string`  }\>

#### Returns

`Promise`<{ `address`: `string` ; `chainCode?`: `string` ; `publicKey`: `string`  }\>

#### Defined in

[evm-ledger/lib/EvmLedgerProvider.ts:83](https://github.com/liquality/chainify/blob/540cfa69/packages/evm-ledger/lib/EvmLedgerProvider.ts#L83)

___

### getNamingProvider

▸ **getNamingProvider**(): `NamingProvider`

#### Returns

`NamingProvider`

#### Inherited from

EvmBaseWalletProvider.getNamingProvider

#### Defined in

client/dist/lib/Wallet.d.ts:10

___

### getSigner

▸ **getSigner**(): [`EvmLedgerSigner`](chainify_evm_ledger.EvmLedgerSigner.md)

#### Returns

[`EvmLedgerSigner`](chainify_evm_ledger.EvmLedgerSigner.md)

#### Inherited from

EvmBaseWalletProvider.getSigner

#### Defined in

evm/dist/lib/wallet/EvmBaseWalletProvider.d.ts:9

___

### getUnusedAddress

▸ **getUnusedAddress**(): `Promise`<`Address`\>

#### Returns

`Promise`<`Address`\>

#### Overrides

EvmBaseWalletProvider.getUnusedAddress

#### Defined in

[evm-ledger/lib/EvmLedgerProvider.ts:62](https://github.com/liquality/chainify/blob/540cfa69/packages/evm-ledger/lib/EvmLedgerProvider.ts#L62)

___

### getUsedAddresses

▸ **getUsedAddresses**(): `Promise`<`Address`[]\>

#### Returns

`Promise`<`Address`[]\>

#### Overrides

EvmBaseWalletProvider.getUsedAddresses

#### Defined in

[evm-ledger/lib/EvmLedgerProvider.ts:66](https://github.com/liquality/chainify/blob/540cfa69/packages/evm-ledger/lib/EvmLedgerProvider.ts#L66)

___

### isWalletAvailable

▸ **isWalletAvailable**(): `Promise`<`boolean`\>

#### Returns

`Promise`<`boolean`\>

#### Overrides

EvmBaseWalletProvider.isWalletAvailable

#### Defined in

[evm-ledger/lib/EvmLedgerProvider.ts:96](https://github.com/liquality/chainify/blob/540cfa69/packages/evm-ledger/lib/EvmLedgerProvider.ts#L96)

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

EvmBaseWalletProvider.onChainProviderUpdate

#### Defined in

[evm-ledger/lib/EvmLedgerProvider.ts:53](https://github.com/liquality/chainify/blob/540cfa69/packages/evm-ledger/lib/EvmLedgerProvider.ts#L53)

___

### sendBatchTransaction

▸ **sendBatchTransaction**(`txRequests`): `Promise`<`Transaction`<`TransactionResponse`\>[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txRequests` | `EthereumTransactionRequest`[] |

#### Returns

`Promise`<`Transaction`<`TransactionResponse`\>[]\>

#### Inherited from

EvmBaseWalletProvider.sendBatchTransaction

#### Defined in

evm/dist/lib/wallet/EvmBaseWalletProvider.d.ts:13

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

EvmBaseWalletProvider.sendSweepTransaction

#### Defined in

evm/dist/lib/wallet/EvmBaseWalletProvider.d.ts:14

___

### sendTransaction

▸ **sendTransaction**(`txRequest`): `Promise`<`Transaction`<`TransactionResponse`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txRequest` | `EthereumTransactionRequest` |

#### Returns

`Promise`<`Transaction`<`TransactionResponse`\>\>

#### Inherited from

EvmBaseWalletProvider.sendTransaction

#### Defined in

evm/dist/lib/wallet/EvmBaseWalletProvider.d.ts:12

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

EvmBaseWalletProvider.setChainProvider

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

EvmBaseWalletProvider.setNamingProvider

#### Defined in

client/dist/lib/Wallet.d.ts:9

___

### setSigner

▸ **setSigner**(`signer`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `signer` | [`EvmLedgerSigner`](chainify_evm_ledger.EvmLedgerSigner.md) |

#### Returns

`void`

#### Inherited from

EvmBaseWalletProvider.setSigner

#### Defined in

evm/dist/lib/wallet/EvmBaseWalletProvider.d.ts:10

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

EvmBaseWalletProvider.signMessage

#### Defined in

evm/dist/lib/wallet/EvmBaseWalletProvider.d.ts:11

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

EvmBaseWalletProvider.signTypedData

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

#### Inherited from

EvmBaseWalletProvider.updateTransactionFee

#### Defined in

evm/dist/lib/wallet/EvmBaseWalletProvider.d.ts:15
