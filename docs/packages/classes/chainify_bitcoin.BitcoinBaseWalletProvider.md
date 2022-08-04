---
id: "chainify_bitcoin.BitcoinBaseWalletProvider"
title: "Class: BitcoinBaseWalletProvider<T, S>"
sidebar_label: "BitcoinBaseWalletProvider"
custom_edit_url: null
---

[@chainify/bitcoin](../modules/chainify_bitcoin.md).BitcoinBaseWalletProvider

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md) = `any` |
| `S` | `any` |

## Hierarchy

- `default`<`T`, `S`\>

  ↳ **`BitcoinBaseWalletProvider`**

  ↳↳ [`BitcoinHDWalletProvider`](chainify_bitcoin.BitcoinHDWalletProvider.md)

## Constructors

### constructor

• **new BitcoinBaseWalletProvider**<`T`, `S`\>(`options`, `chainProvider?`)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md)<`T`\> = `any` |
| `S` | `any` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`BitcoinWalletProviderOptions`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinWalletProviderOptions.md) |
| `chainProvider?` | `default`<`T`, `Network`\> |

#### Overrides

Wallet&lt;T, S\&gt;.constructor

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:39](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L39)

## Properties

### \_addressType

• `Protected` **\_addressType**: [`AddressType`](../enums/chainify_bitcoin.BitcoinTypes.AddressType.md)

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:36](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L36)

___

### \_baseDerivationPath

• `Protected` **\_baseDerivationPath**: `string`

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:34](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L34)

___

### \_derivationCache

• `Protected` **\_derivationCache**: `DerivationCache`

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:37](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L37)

___

### \_network

• `Protected` **\_network**: [`BitcoinNetwork`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinNetwork.md)

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:35](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L35)

___

### chainProvider

• `Protected` **chainProvider**: `default`<`T`, `Network`\>

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

### \_getUsedUnusedAddresses

▸ `Protected` **_getUsedUnusedAddresses**(`numAddressPerCall?`, `addressType`): `Promise`<{ `unusedAddress`: { `change`: `Address` ; `external`: `Address`  } = unusedAddressMap; `usedAddresses`: `Address`[]  }\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `numAddressPerCall` | `number` | `100` |
| `addressType` | `AddressSearchType` | `undefined` |

#### Returns

`Promise`<{ `unusedAddress`: { `change`: `Address` ; `external`: `Address`  } = unusedAddressMap; `usedAddresses`: `Address`[]  }\>

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:215](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L215)

___

### \_sendTransaction

▸ `Protected` **_sendTransaction**(`transactions`, `feePerByte?`): `Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `transactions` | [`OutputTarget`](../interfaces/chainify_bitcoin.BitcoinTypes.OutputTarget.md)[] |
| `feePerByte?` | `number` |

#### Returns

`Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:161](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L161)

___

### baseDerivationNode

▸ `Protected` `Abstract` **baseDerivationNode**(): `Promise`<`BIP32Interface`\>

#### Returns

`Promise`<`BIP32Interface`\>

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:58](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L58)

___

### buildSweepTransaction

▸ `Protected` `Abstract` **buildSweepTransaction**(`externalChangeAddress`, `feePerByte?`): `Promise`<{ `fee`: `number` ; `hex`: `string`  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `externalChangeAddress` | `string` |
| `feePerByte?` | `number` |

#### Returns

`Promise`<{ `fee`: `number` ; `hex`: `string`  }\>

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:64](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L64)

___

### buildTransaction

▸ `Protected` `Abstract` **buildTransaction**(`targets`, `feePerByte?`, `fixedInputs?`): `Promise`<{ `fee`: `number` ; `hex`: `string`  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `targets` | [`OutputTarget`](../interfaces/chainify_bitcoin.BitcoinTypes.OutputTarget.md)[] |
| `feePerByte?` | `number` |
| `fixedInputs?` | [`Input`](../interfaces/chainify_bitcoin.BitcoinTypes.Input.md)[] |

#### Returns

`Promise`<{ `fee`: `number` ; `hex`: `string`  }\>

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:59](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L59)

___

### canUpdateFee

▸ `Abstract` **canUpdateFee**(): `boolean`

#### Returns

`boolean`

#### Inherited from

Wallet.canUpdateFee

#### Defined in

client/dist/lib/Wallet.d.ts:26

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

### findAddress

▸ `Protected` **findAddress**(`addresses`, `change?`): `Promise`<`Address`\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `addresses` | `string`[] | `undefined` |
| `change` | `boolean` | `false` |

#### Returns

`Promise`<`Address`\>

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:167](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L167)

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

### getAddressFromPublicKey

▸ `Protected` **getAddressFromPublicKey**(`publicKey`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | `Buffer` |

#### Returns

`string`

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:466](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L466)

___

### getAddresses

▸ **getAddresses**(`startingIndex?`, `numAddresses?`, `change?`): `Promise`<`Address`[]\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `startingIndex` | `number` | `0` |
| `numAddresses` | `number` | `1` |
| `change` | `boolean` | `false` |

#### Returns

`Promise`<`Address`[]\>

#### Overrides

Wallet.getAddresses

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:90](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L90)

___

### getBalance

▸ `Abstract` **getBalance**(`assets`): `Promise`<`BigNumber`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `assets` | `Asset`[] |

#### Returns

`Promise`<`BigNumber`[]\>

#### Inherited from

Wallet.getBalance

#### Defined in

client/dist/lib/Wallet.d.ts:23

___

### getChainProvider

▸ **getChainProvider**(): `default`<`T`, `Network`\>

#### Returns

`default`<`T`, `Network`\>

#### Inherited from

Wallet.getChainProvider

#### Defined in

client/dist/lib/Wallet.d.ts:8

___

### getConnectedNetwork

▸ `Abstract` **getConnectedNetwork**(): `Promise`<`Network`\>

#### Returns

`Promise`<`Network`\>

#### Inherited from

Wallet.getConnectedNetwork

#### Defined in

client/dist/lib/Wallet.d.ts:12

___

### getDerivationCache

▸ **getDerivationCache**(): `DerivationCache`

#### Returns

`DerivationCache`

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:74](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L74)

___

### getDerivationPathAddress

▸ `Protected` **getDerivationPathAddress**(`path`): `Promise`<`Address`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `path` | `string` |

#### Returns

`Promise`<`Address`\>

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:196](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L196)

___

### getInputsForAmount

▸ `Protected` **getInputsForAmount**(`_targets`, `feePerByte?`, `fixedInputs?`, `numAddressPerCall?`, `sweep?`): `Promise`<{ `change`: [`CoinSelectTarget`](../namespaces/chainify_bitcoin.BitcoinUtils.md#coinselecttarget) ; `fee`: `number` ; `inputs`: [`UTXO`](../interfaces/chainify_bitcoin.BitcoinTypes.UTXO.md)[] ; `outputs`: [`CoinSelectTarget`](../namespaces/chainify_bitcoin.BitcoinUtils.md#coinselecttarget)[]  }\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `_targets` | [`OutputTarget`](../interfaces/chainify_bitcoin.BitcoinTypes.OutputTarget.md)[] | `undefined` |
| `feePerByte?` | `number` | `undefined` |
| `fixedInputs` | [`Input`](../interfaces/chainify_bitcoin.BitcoinTypes.Input.md)[] | `[]` |
| `numAddressPerCall` | `number` | `100` |
| `sweep` | `boolean` | `false` |

#### Returns

`Promise`<{ `change`: [`CoinSelectTarget`](../namespaces/chainify_bitcoin.BitcoinUtils.md#coinselecttarget) ; `fee`: `number` ; `inputs`: [`UTXO`](../interfaces/chainify_bitcoin.BitcoinTypes.UTXO.md)[] ; `outputs`: [`CoinSelectTarget`](../namespaces/chainify_bitcoin.BitcoinUtils.md#coinselecttarget)[]  }\>

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:319](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L319)

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

### getPaymentVariantFromPublicKey

▸ `Protected` **getPaymentVariantFromPublicKey**(`publicKey`): `Payment`

#### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | `Buffer` |

#### Returns

`Payment`

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:470](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L470)

___

### getSigner

▸ `Abstract` **getSigner**(): `S`

#### Returns

`S`

#### Inherited from

Wallet.getSigner

#### Defined in

client/dist/lib/Wallet.d.ts:13

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

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:302](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L302)

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

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:149](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L149)

___

### getUnusedAddress

▸ **getUnusedAddress**(`change?`, `numAddressPerCall?`): `Promise`<`Address`\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `change` | `boolean` | `false` |
| `numAddressPerCall` | `number` | `100` |

#### Returns

`Promise`<`Address`\>

#### Overrides

Wallet.getUnusedAddress

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:78](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L78)

___

### getUsedAddresses

▸ **getUsedAddresses**(`numAddressPerCall?`): `Promise`<`Address`[]\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `numAddressPerCall` | `number` | `100` |

#### Returns

`Promise`<`Address`[]\>

#### Overrides

Wallet.getUsedAddresses

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:84](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L84)

___

### getWalletAddress

▸ **getWalletAddress**(`address`): `Promise`<`Address`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |

#### Returns

`Promise`<`Address`\>

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:182](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L182)

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

▸ `Protected` **onChainProviderUpdate**(`chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider` | `default`<`T`, `Network`\> |

#### Returns

`void`

#### Overrides

Wallet.onChainProviderUpdate

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:54](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L54)

___

### sendBatchTransaction

▸ **sendBatchTransaction**(`transactions`): `Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `transactions` | `TransactionRequest`[] |

#### Returns

`Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>[]\>

#### Overrides

Wallet.sendBatchTransaction

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:115](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L115)

___

### sendOptionsToOutputs

▸ `Protected` **sendOptionsToOutputs**(`transactions`): [`OutputTarget`](../interfaces/chainify_bitcoin.BitcoinTypes.OutputTarget.md)[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `transactions` | `TransactionRequest`[] |

#### Returns

[`OutputTarget`](../interfaces/chainify_bitcoin.BitcoinTypes.OutputTarget.md)[]

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:443](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L443)

___

### sendSweepTransaction

▸ **sendSweepTransaction**(`externalChangeAddress`, `_asset`, `feePerByte`): `Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `externalChangeAddress` | `AddressType` |
| `_asset` | `Asset` |
| `feePerByte` | `number` |

#### Returns

`Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Overrides

Wallet.sendSweepTransaction

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:119](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L119)

___

### sendTransaction

▸ **sendTransaction**(`options`): `Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | `TransactionRequest` |

#### Returns

`Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Overrides

Wallet.sendTransaction

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:111](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L111)

___

### setChainProvider

▸ **setChainProvider**(`chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider` | `default`<`T`, `Network`\> |

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

### signBatchP2SHTransaction

▸ `Abstract` **signBatchP2SHTransaction**(`inputs`, `addresses`, `tx`, `lockTime?`, `segwit?`): `Promise`<`Buffer`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `inputs` | [`P2SHInput`](../interfaces/chainify_bitcoin.BitcoinTypes.P2SHInput.md)[] |
| `addresses` | `string` |
| `tx` | `any` |
| `lockTime?` | `number` |
| `segwit?` | `boolean` |

#### Returns

`Promise`<`Buffer`[]\>

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:66](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L66)

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

#### Inherited from

Wallet.signMessage

#### Defined in

client/dist/lib/Wallet.d.ts:18

___

### signPSBT

▸ `Abstract` **signPSBT**(`data`, `inputs`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | `string` |
| `inputs` | [`PsbtInputTarget`](../interfaces/chainify_bitcoin.BitcoinTypes.PsbtInputTarget.md)[] |

#### Returns

`Promise`<`string`\>

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:65](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L65)

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

▸ **updateTransactionFee**(`tx`, `newFeePerByte`): `Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `tx` | `string` \| `Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\> |
| `newFeePerByte` | `number` |

#### Returns

`Promise`<`Transaction`<[`Transaction`](../interfaces/chainify_bitcoin.BitcoinTypes.Transaction.md)\>\>

#### Overrides

Wallet.updateTransactionFee

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:125](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L125)

___

### withCachedUtxos

▸ `Protected` **withCachedUtxos**(`func`): `Promise`<`any`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `func` | () => `any` |

#### Returns

`Promise`<`any`\>

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:284](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L284)
