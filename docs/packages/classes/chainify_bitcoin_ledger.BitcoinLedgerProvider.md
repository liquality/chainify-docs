---
id: "chainify_bitcoin_ledger.BitcoinLedgerProvider"
title: "Class: BitcoinLedgerProvider"
sidebar_label: "BitcoinLedgerProvider"
custom_edit_url: null
---

[@chainify/bitcoin-ledger](../modules/chainify_bitcoin_ledger.md).BitcoinLedgerProvider

## Hierarchy

- `BitcoinBaseWalletProvider`

  ↳ **`BitcoinLedgerProvider`**

## Constructors

### constructor

• **new BitcoinLedgerProvider**(`options`, `chainProvider`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`BitcoinLedgerProviderOptions`](../interfaces/chainify_bitcoin_ledger.BitcoinLedgerProviderTypes.BitcoinLedgerProviderOptions.md) |
| `chainProvider` | `default`<`BitcoinBaseChainProvider`, `Network`\> |

#### Overrides

BitcoinBaseWalletProvider.constructor

#### Defined in

[bitcoin-ledger/lib/BitcoinLedgerProvider.ts:17](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/BitcoinLedgerProvider.ts#L17)

## Properties

### \_addressType

• `Protected` **\_addressType**: `AddressType`

#### Inherited from

BitcoinBaseWalletProvider.\_addressType

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:20

___

### \_baseDerivationPath

• `Protected` **\_baseDerivationPath**: `string`

#### Inherited from

BitcoinBaseWalletProvider.\_baseDerivationPath

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:18

___

### \_derivationCache

• `Protected` **\_derivationCache**: `DerivationCache`

#### Inherited from

BitcoinBaseWalletProvider.\_derivationCache

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:21

___

### \_network

• `Protected` **\_network**: `BitcoinNetwork`

#### Inherited from

BitcoinBaseWalletProvider.\_network

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:19

___

### chainProvider

• `Protected` **chainProvider**: `default`<`any`, `Network`\>

#### Inherited from

BitcoinBaseWalletProvider.chainProvider

#### Defined in

client/dist/lib/Wallet.d.ts:4

___

### namingProvider

• `Protected` **namingProvider**: `NamingProvider`

#### Inherited from

BitcoinBaseWalletProvider.namingProvider

#### Defined in

client/dist/lib/Wallet.d.ts:5

## Methods

### \_getUsedUnusedAddresses

▸ `Protected` **_getUsedUnusedAddresses**(`numAddressPerCall`, `addressType`): `Promise`<{ `unusedAddress`: { `change`: `Address` ; `external`: `Address`  } ; `usedAddresses`: `Address`[]  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `numAddressPerCall` | `number` |
| `addressType` | `AddressSearchType` |

#### Returns

`Promise`<{ `unusedAddress`: { `change`: `Address` ; `external`: `Address`  } ; `usedAddresses`: `Address`[]  }\>

#### Inherited from

BitcoinBaseWalletProvider.\_getUsedUnusedAddresses

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:48

___

### \_sendTransaction

▸ `Protected` **_sendTransaction**(`transactions`, `feePerByte?`): `Promise`<`Transaction`<`Transaction`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `transactions` | `OutputTarget`[] |
| `feePerByte?` | `number` |

#### Returns

`Promise`<`Transaction`<`Transaction`\>\>

#### Inherited from

BitcoinBaseWalletProvider.\_sendTransaction

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:44

___

### baseDerivationNode

▸ `Protected` **baseDerivationNode**(): `Promise`<`BIP32Interface`\>

#### Returns

`Promise`<`BIP32Interface`\>

#### Overrides

BitcoinBaseWalletProvider.baseDerivationNode

#### Defined in

[bitcoin-ledger/lib/BitcoinLedgerProvider.ts:263](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/BitcoinLedgerProvider.ts#L263)

___

### buildSweepTransaction

▸ `Protected` **buildSweepTransaction**(`_externalChangeAddress`, `_feePerByte?`): `Promise`<{ `fee`: `number` ; `hex`: `string`  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_externalChangeAddress` | `string` |
| `_feePerByte?` | `number` |

#### Returns

`Promise`<{ `fee`: `number` ; `hex`: `string`  }\>

#### Overrides

BitcoinBaseWalletProvider.buildSweepTransaction

#### Defined in

[bitcoin-ledger/lib/BitcoinLedgerProvider.ts:259](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/BitcoinLedgerProvider.ts#L259)

___

### buildTransaction

▸ `Protected` **buildTransaction**(`targets`, `feePerByte?`, `fixedInputs?`): `Promise`<{ `fee`: `number` ; `hex`: `string`  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `targets` | `OutputTarget`[] |
| `feePerByte?` | `number` |
| `fixedInputs?` | `Input`[] |

#### Returns

`Promise`<{ `fee`: `number` ; `hex`: `string`  }\>

#### Overrides

BitcoinBaseWalletProvider.buildTransaction

#### Defined in

[bitcoin-ledger/lib/BitcoinLedgerProvider.ts:277](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/BitcoinLedgerProvider.ts#L277)

___

### canUpdateFee

▸ **canUpdateFee**(): `boolean`

#### Returns

`boolean`

#### Overrides

BitcoinBaseWalletProvider.canUpdateFee

#### Defined in

[bitcoin-ledger/lib/BitcoinLedgerProvider.ts:70](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/BitcoinLedgerProvider.ts#L70)

___

### exportPrivateKey

▸ **exportPrivateKey**(): `Promise`<`string`\>

#### Returns

`Promise`<`string`\>

#### Overrides

BitcoinBaseWalletProvider.exportPrivateKey

#### Defined in

[bitcoin-ledger/lib/BitcoinLedgerProvider.ts:62](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/BitcoinLedgerProvider.ts#L62)

___

### findAddress

▸ `Protected` **findAddress**(`addresses`, `change?`): `Promise`<`Address`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `addresses` | `string`[] |
| `change?` | `boolean` |

#### Returns

`Promise`<`Address`\>

#### Inherited from

BitcoinBaseWalletProvider.findAddress

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:45

___

### getAddress

▸ **getAddress**(): `Promise`<`AddressType`\>

#### Returns

`Promise`<`AddressType`\>

#### Overrides

BitcoinBaseWalletProvider.getAddress

#### Defined in

[bitcoin-ledger/lib/BitcoinLedgerProvider.ts:52](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/BitcoinLedgerProvider.ts#L52)

___

### getAddressFromPublicKey

▸ `Protected` **getAddressFromPublicKey**(`publicKey`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | `Buffer` |

#### Returns

`string`

#### Inherited from

BitcoinBaseWalletProvider.getAddressFromPublicKey

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:64

___

### getAddresses

▸ **getAddresses**(`startingIndex?`, `numAddresses?`, `change?`): `Promise`<`Address`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `startingIndex?` | `number` |
| `numAddresses?` | `number` |
| `change?` | `boolean` |

#### Returns

`Promise`<`Address`[]\>

#### Inherited from

BitcoinBaseWalletProvider.getAddresses

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:38

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

BitcoinBaseWalletProvider.getBalance

#### Defined in

[bitcoin-ledger/lib/BitcoinLedgerProvider.ts:57](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/BitcoinLedgerProvider.ts#L57)

___

### getChainProvider

▸ **getChainProvider**(): `default`<`any`, `Network`\>

#### Returns

`default`<`any`, `Network`\>

#### Inherited from

BitcoinBaseWalletProvider.getChainProvider

#### Defined in

client/dist/lib/Wallet.d.ts:8

___

### getConnectedNetwork

▸ **getConnectedNetwork**(): `Promise`<`Network`\>

#### Returns

`Promise`<`Network`\>

#### Overrides

BitcoinBaseWalletProvider.getConnectedNetwork

#### Defined in

[bitcoin-ledger/lib/BitcoinLedgerProvider.ts:44](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/BitcoinLedgerProvider.ts#L44)

___

### getDerivationCache

▸ **getDerivationCache**(): `DerivationCache`

#### Returns

`DerivationCache`

#### Inherited from

BitcoinBaseWalletProvider.getDerivationCache

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:35

___

### getDerivationPathAddress

▸ `Protected` **getDerivationPathAddress**(`path`): `Promise`<`Address`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `path` | `string` |

#### Returns

`Promise`<`Address`\>

#### Inherited from

BitcoinBaseWalletProvider.getDerivationPathAddress

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:47

___

### getInputsForAmount

▸ `Protected` **getInputsForAmount**(`_targets`, `feePerByte?`, `fixedInputs?`, `numAddressPerCall?`, `sweep?`): `Promise`<{ `change`: `CoinSelectTarget` ; `fee`: `number` ; `inputs`: `UTXO`[] ; `outputs`: `CoinSelectTarget`[]  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_targets` | `OutputTarget`[] |
| `feePerByte?` | `number` |
| `fixedInputs?` | `Input`[] |
| `numAddressPerCall?` | `number` |
| `sweep?` | `boolean` |

#### Returns

`Promise`<{ `change`: `CoinSelectTarget` ; `fee`: `number` ; `inputs`: `UTXO`[] ; `outputs`: `CoinSelectTarget`[]  }\>

#### Inherited from

BitcoinBaseWalletProvider.getInputsForAmount

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:57

___

### getNamingProvider

▸ **getNamingProvider**(): `NamingProvider`

#### Returns

`NamingProvider`

#### Inherited from

BitcoinBaseWalletProvider.getNamingProvider

#### Defined in

client/dist/lib/Wallet.d.ts:10

___

### getPaymentVariantFromPublicKey

▸ `Protected` **getPaymentVariantFromPublicKey**(`publicKey`): `Payment`

#### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | `Buffer` |

#### Returns

`Payment`

#### Inherited from

BitcoinBaseWalletProvider.getPaymentVariantFromPublicKey

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:65

___

### getSigner

▸ **getSigner**(): `Promise`<``null``\>

#### Returns

`Promise`<``null``\>

#### Overrides

BitcoinBaseWalletProvider.getSigner

#### Defined in

[bitcoin-ledger/lib/BitcoinLedgerProvider.ts:48](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/BitcoinLedgerProvider.ts#L48)

___

### getTotalFee

▸ `Protected` **getTotalFee**(`opts`, `max`): `Promise`<`number`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `opts` | `TransactionRequest` |
| `max` | `boolean` |

#### Returns

`Promise`<`number`\>

#### Inherited from

BitcoinBaseWalletProvider.getTotalFee

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:56

___

### getTotalFees

▸ **getTotalFees**(`transactions`, `max`): `Promise`<`any`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `transactions` | `TransactionRequest`[] |
| `max` | `boolean` |

#### Returns

`Promise`<`any`\>

#### Inherited from

BitcoinBaseWalletProvider.getTotalFees

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:43

___

### getUnusedAddress

▸ **getUnusedAddress**(`change?`, `numAddressPerCall?`): `Promise`<`Address`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `change?` | `boolean` |
| `numAddressPerCall?` | `number` |

#### Returns

`Promise`<`Address`\>

#### Inherited from

BitcoinBaseWalletProvider.getUnusedAddress

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:36

___

### getUsedAddresses

▸ **getUsedAddresses**(`numAddressPerCall?`): `Promise`<`Address`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `numAddressPerCall?` | `number` |

#### Returns

`Promise`<`Address`[]\>

#### Inherited from

BitcoinBaseWalletProvider.getUsedAddresses

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:37

___

### getWalletAddress

▸ **getWalletAddress**(`address`): `Promise`<`Address`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |

#### Returns

`Promise`<`Address`\>

#### Inherited from

BitcoinBaseWalletProvider.getWalletAddress

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:46

___

### getWalletPublicKey

▸ **getWalletPublicKey**(`path`): `Promise`<`any`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `path` | `string` |

#### Returns

`Promise`<`any`\>

#### Defined in

[bitcoin-ledger/lib/BitcoinLedgerProvider.ts:249](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/BitcoinLedgerProvider.ts#L249)

___

### isWalletAvailable

▸ **isWalletAvailable**(): `Promise`<`boolean`\>

#### Returns

`Promise`<`boolean`\>

#### Overrides

BitcoinBaseWalletProvider.isWalletAvailable

#### Defined in

[bitcoin-ledger/lib/BitcoinLedgerProvider.ts:66](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/BitcoinLedgerProvider.ts#L66)

___

### onChainProviderUpdate

▸ `Protected` **onChainProviderUpdate**(`chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider` | `default`<`any`, `Network`\> |

#### Returns

`void`

#### Inherited from

BitcoinBaseWalletProvider.onChainProviderUpdate

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:23

___

### sendBatchTransaction

▸ **sendBatchTransaction**(`transactions`): `Promise`<`Transaction`<`Transaction`\>[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `transactions` | `TransactionRequest`[] |

#### Returns

`Promise`<`Transaction`<`Transaction`\>[]\>

#### Inherited from

BitcoinBaseWalletProvider.sendBatchTransaction

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:40

___

### sendOptionsToOutputs

▸ `Protected` **sendOptionsToOutputs**(`transactions`): `OutputTarget`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `transactions` | `TransactionRequest`[] |

#### Returns

`OutputTarget`[]

#### Inherited from

BitcoinBaseWalletProvider.sendOptionsToOutputs

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:63

___

### sendSweepTransaction

▸ **sendSweepTransaction**(`externalChangeAddress`, `_asset`, `feePerByte`): `Promise`<`Transaction`<`Transaction`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `externalChangeAddress` | `AddressType` |
| `_asset` | `Asset` |
| `feePerByte` | `number` |

#### Returns

`Promise`<`Transaction`<`Transaction`\>\>

#### Inherited from

BitcoinBaseWalletProvider.sendSweepTransaction

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:41

___

### sendTransaction

▸ **sendTransaction**(`options`): `Promise`<`Transaction`<`Transaction`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | `TransactionRequest` |

#### Returns

`Promise`<`Transaction`<`Transaction`\>\>

#### Inherited from

BitcoinBaseWalletProvider.sendTransaction

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:39

___

### setChainProvider

▸ **setChainProvider**(`chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider` | `default`<`any`, `Network`\> |

#### Returns

`void`

#### Inherited from

BitcoinBaseWalletProvider.setChainProvider

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

BitcoinBaseWalletProvider.setNamingProvider

#### Defined in

client/dist/lib/Wallet.d.ts:9

___

### signBatchP2SHTransaction

▸ **signBatchP2SHTransaction**(`inputs`, `addresses`, `tx`, `lockTime?`, `segwit?`): `Promise`<`Buffer`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `inputs` | [{ `index`: `number` ; `inputTxHex`: `string` ; `outputScript`: `Buffer` ; `vout`: `any`  }] |
| `addresses` | `string` |
| `tx` | `any` |
| `lockTime?` | `number` |
| `segwit?` | `boolean` |

#### Returns

`Promise`<`Buffer`[]\>

#### Overrides

BitcoinBaseWalletProvider.signBatchP2SHTransaction

#### Defined in

[bitcoin-ledger/lib/BitcoinLedgerProvider.ts:199](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/BitcoinLedgerProvider.ts#L199)

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

#### Overrides

BitcoinBaseWalletProvider.signMessage

#### Defined in

[bitcoin-ledger/lib/BitcoinLedgerProvider.ts:36](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/BitcoinLedgerProvider.ts#L36)

___

### signPSBT

▸ **signPSBT**(`data`, `inputs`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | `string` |
| `inputs` | `PsbtInputTarget`[] |

#### Returns

`Promise`<`string`\>

#### Overrides

BitcoinBaseWalletProvider.signPSBT

#### Defined in

[bitcoin-ledger/lib/BitcoinLedgerProvider.ts:74](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin-ledger/lib/BitcoinLedgerProvider.ts#L74)

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

BitcoinBaseWalletProvider.signTypedData

#### Defined in

client/dist/lib/Wallet.d.ts:11

___

### updateTransactionFee

▸ **updateTransactionFee**(`tx`, `newFeePerByte`): `Promise`<`Transaction`<`Transaction`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `tx` | `string` \| `Transaction`<`Transaction`\> |
| `newFeePerByte` | `number` |

#### Returns

`Promise`<`Transaction`<`Transaction`\>\>

#### Inherited from

BitcoinBaseWalletProvider.updateTransactionFee

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:42

___

### withCachedUtxos

▸ `Protected` **withCachedUtxos**(`func`): `Promise`<`any`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `func` | () => `any` |

#### Returns

`Promise`<`any`\>

#### Inherited from

BitcoinBaseWalletProvider.withCachedUtxos

#### Defined in

bitcoin/dist/lib/wallet/BitcoinBaseWallet.d.ts:55
