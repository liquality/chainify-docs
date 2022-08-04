---
id: "chainify_bitcoin.BitcoinHDWalletProvider"
title: "Class: BitcoinHDWalletProvider"
sidebar_label: "BitcoinHDWalletProvider"
custom_edit_url: null
---

[@chainify/bitcoin](../modules/chainify_bitcoin.md).BitcoinHDWalletProvider

## Hierarchy

- [`BitcoinBaseWalletProvider`](chainify_bitcoin.BitcoinBaseWalletProvider.md)

  ↳ **`BitcoinHDWalletProvider`**

## Implements

- `IBitcoinWallet`<[`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md)\>

## Constructors

### constructor

• **new BitcoinHDWalletProvider**(`options`, `chainProvider?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`BitcoinHDWalletProviderOptions`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinHDWalletProviderOptions.md) |
| `chainProvider?` | `default`<[`BitcoinBaseChainProvider`](chainify_bitcoin.BitcoinBaseChainProvider.md), `Network`\> |

#### Overrides

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[constructor](chainify_bitcoin.BitcoinBaseWalletProvider.md#constructor)

#### Defined in

[bitcoin/lib/wallet/BitcoinHDWallet.ts:17](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinHDWallet.ts#L17)

## Properties

### \_addressType

• `Protected` **\_addressType**: [`AddressType`](../enums/chainify_bitcoin.BitcoinTypes.AddressType.md)

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[_addressType](chainify_bitcoin.BitcoinBaseWalletProvider.md#_addresstype)

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:36](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L36)

___

### \_baseDerivationPath

• `Protected` **\_baseDerivationPath**: `string`

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[_baseDerivationPath](chainify_bitcoin.BitcoinBaseWalletProvider.md#_basederivationpath)

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:34](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L34)

___

### \_derivationCache

• `Protected` **\_derivationCache**: `DerivationCache`

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[_derivationCache](chainify_bitcoin.BitcoinBaseWalletProvider.md#_derivationcache)

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:37](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L37)

___

### \_network

• `Protected` **\_network**: [`BitcoinNetwork`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinNetwork.md)

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[_network](chainify_bitcoin.BitcoinBaseWalletProvider.md#_network)

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:35](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L35)

___

### chainProvider

• `Protected` **chainProvider**: `default`<`any`, `Network`\>

#### Implementation of

IBitcoinWallet.chainProvider

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[chainProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md#chainprovider)

#### Defined in

client/dist/lib/Wallet.d.ts:4

___

### namingProvider

• `Protected` **namingProvider**: `NamingProvider`

#### Implementation of

IBitcoinWallet.namingProvider

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[namingProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md#namingprovider)

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

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[_getUsedUnusedAddresses](chainify_bitcoin.BitcoinBaseWalletProvider.md#_getusedunusedaddresses)

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

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[_sendTransaction](chainify_bitcoin.BitcoinBaseWalletProvider.md#_sendtransaction)

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:161](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L161)

___

### baseDerivationNode

▸ `Protected` **baseDerivationNode**(): `Promise`<`BIP32Interface`\>

#### Returns

`Promise`<`BIP32Interface`\>

#### Overrides

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[baseDerivationNode](chainify_bitcoin.BitcoinBaseWalletProvider.md#basederivationnode)

#### Defined in

[bitcoin/lib/wallet/BitcoinHDWallet.ts:64](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinHDWallet.ts#L64)

___

### buildSweepTransaction

▸ `Protected` **buildSweepTransaction**(`externalChangeAddress`, `feePerByte`): `Promise`<{ `fee`: `number` ; `hex`: `string`  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `externalChangeAddress` | `string` |
| `feePerByte` | `number` |

#### Returns

`Promise`<{ `fee`: `number` ; `hex`: `string`  }\>

#### Overrides

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[buildSweepTransaction](chainify_bitcoin.BitcoinBaseWalletProvider.md#buildsweeptransaction)

#### Defined in

[bitcoin/lib/wallet/BitcoinHDWallet.ts:144](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinHDWallet.ts#L144)

___

### buildTransaction

▸ `Protected` **buildTransaction**(`targets`, `feePerByte?`, `fixedInputs?`): `Promise`<{ `fee`: `number` ; `hex`: `string`  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `targets` | [`OutputTarget`](../interfaces/chainify_bitcoin.BitcoinTypes.OutputTarget.md)[] |
| `feePerByte?` | `number` |
| `fixedInputs?` | [`Input`](../interfaces/chainify_bitcoin.BitcoinTypes.Input.md)[] |

#### Returns

`Promise`<{ `fee`: `number` ; `hex`: `string`  }\>

#### Overrides

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[buildTransaction](chainify_bitcoin.BitcoinBaseWalletProvider.md#buildtransaction)

#### Defined in

[bitcoin/lib/wallet/BitcoinHDWallet.ts:73](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinHDWallet.ts#L73)

___

### canUpdateFee

▸ **canUpdateFee**(): `boolean`

#### Returns

`boolean`

#### Implementation of

IBitcoinWallet.canUpdateFee

#### Overrides

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[canUpdateFee](chainify_bitcoin.BitcoinBaseWalletProvider.md#canupdatefee)

#### Defined in

[bitcoin/lib/wallet/BitcoinHDWallet.ts:27](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinHDWallet.ts#L27)

___

### exportPrivateKey

▸ **exportPrivateKey**(): `Promise`<`string`\>

#### Returns

`Promise`<`string`\>

#### Implementation of

IBitcoinWallet.exportPrivateKey

#### Overrides

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[exportPrivateKey](chainify_bitcoin.BitcoinBaseWalletProvider.md#exportprivatekey)

#### Defined in

[bitcoin/lib/wallet/BitcoinHDWallet.ts:52](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinHDWallet.ts#L52)

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

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[findAddress](chainify_bitcoin.BitcoinBaseWalletProvider.md#findaddress)

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:167](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L167)

___

### getAddress

▸ **getAddress**(): `Promise`<`AddressType`\>

#### Returns

`Promise`<`AddressType`\>

#### Implementation of

IBitcoinWallet.getAddress

#### Overrides

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[getAddress](chainify_bitcoin.BitcoinBaseWalletProvider.md#getaddress)

#### Defined in

[bitcoin/lib/wallet/BitcoinHDWallet.ts:35](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinHDWallet.ts#L35)

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

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[getAddressFromPublicKey](chainify_bitcoin.BitcoinBaseWalletProvider.md#getaddressfrompublickey)

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

#### Implementation of

IBitcoinWallet.getAddresses

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[getAddresses](chainify_bitcoin.BitcoinBaseWalletProvider.md#getaddresses)

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:90](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L90)

___

### getBalance

▸ **getBalance**(`_assets`): `Promise`<`BigNumber`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_assets` | `Asset`[] |

#### Returns

`Promise`<`BigNumber`[]\>

#### Implementation of

IBitcoinWallet.getBalance

#### Overrides

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[getBalance](chainify_bitcoin.BitcoinBaseWalletProvider.md#getbalance)

#### Defined in

[bitcoin/lib/wallet/BitcoinHDWallet.ts:40](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinHDWallet.ts#L40)

___

### getChainProvider

▸ **getChainProvider**(): `default`<`any`, `Network`\>

#### Returns

`default`<`any`, `Network`\>

#### Implementation of

IBitcoinWallet.getChainProvider

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[getChainProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md#getchainprovider)

#### Defined in

client/dist/lib/Wallet.d.ts:8

___

### getConnectedNetwork

▸ **getConnectedNetwork**(): `Promise`<[`BitcoinNetwork`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinNetwork.md)\>

#### Returns

`Promise`<[`BitcoinNetwork`](../interfaces/chainify_bitcoin.BitcoinTypes.BitcoinNetwork.md)\>

#### Implementation of

IBitcoinWallet.getConnectedNetwork

#### Overrides

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[getConnectedNetwork](chainify_bitcoin.BitcoinBaseWalletProvider.md#getconnectednetwork)

#### Defined in

[bitcoin/lib/wallet/BitcoinHDWallet.ts:56](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinHDWallet.ts#L56)

___

### getDerivationCache

▸ **getDerivationCache**(): `DerivationCache`

#### Returns

`DerivationCache`

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[getDerivationCache](chainify_bitcoin.BitcoinBaseWalletProvider.md#getderivationcache)

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

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[getDerivationPathAddress](chainify_bitcoin.BitcoinBaseWalletProvider.md#getderivationpathaddress)

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

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[getInputsForAmount](chainify_bitcoin.BitcoinBaseWalletProvider.md#getinputsforamount)

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:319](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L319)

___

### getNamingProvider

▸ **getNamingProvider**(): `NamingProvider`

#### Returns

`NamingProvider`

#### Implementation of

IBitcoinWallet.getNamingProvider

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[getNamingProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md#getnamingprovider)

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

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[getPaymentVariantFromPublicKey](chainify_bitcoin.BitcoinBaseWalletProvider.md#getpaymentvariantfrompublickey)

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:470](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L470)

___

### getSigner

▸ **getSigner**(): `Promise`<``null``\>

#### Returns

`Promise`<``null``\>

#### Implementation of

IBitcoinWallet.getSigner

#### Overrides

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[getSigner](chainify_bitcoin.BitcoinBaseWalletProvider.md#getsigner)

#### Defined in

[bitcoin/lib/wallet/BitcoinHDWallet.ts:31](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinHDWallet.ts#L31)

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

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[getTotalFee](chainify_bitcoin.BitcoinBaseWalletProvider.md#gettotalfee)

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

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[getTotalFees](chainify_bitcoin.BitcoinBaseWalletProvider.md#gettotalfees)

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

#### Implementation of

IBitcoinWallet.getUnusedAddress

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[getUnusedAddress](chainify_bitcoin.BitcoinBaseWalletProvider.md#getunusedaddress)

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

#### Implementation of

IBitcoinWallet.getUsedAddresses

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[getUsedAddresses](chainify_bitcoin.BitcoinBaseWalletProvider.md#getusedaddresses)

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

#### Implementation of

IBitcoinWallet.getWalletAddress

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[getWalletAddress](chainify_bitcoin.BitcoinBaseWalletProvider.md#getwalletaddress)

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:182](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L182)

___

### isWalletAvailable

▸ **isWalletAvailable**(): `Promise`<`boolean`\>

#### Returns

`Promise`<`boolean`\>

#### Implementation of

IBitcoinWallet.isWalletAvailable

#### Overrides

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[isWalletAvailable](chainify_bitcoin.BitcoinBaseWalletProvider.md#iswalletavailable)

#### Defined in

[bitcoin/lib/wallet/BitcoinHDWallet.ts:60](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinHDWallet.ts#L60)

___

### onChainProviderUpdate

▸ `Protected` **onChainProviderUpdate**(`chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider` | `default`<`any`, `Network`\> |

#### Returns

`void`

#### Implementation of

IBitcoinWallet.onChainProviderUpdate

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[onChainProviderUpdate](chainify_bitcoin.BitcoinBaseWalletProvider.md#onchainproviderupdate)

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

#### Implementation of

IBitcoinWallet.sendBatchTransaction

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[sendBatchTransaction](chainify_bitcoin.BitcoinBaseWalletProvider.md#sendbatchtransaction)

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

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[sendOptionsToOutputs](chainify_bitcoin.BitcoinBaseWalletProvider.md#sendoptionstooutputs)

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

#### Implementation of

IBitcoinWallet.sendSweepTransaction

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[sendSweepTransaction](chainify_bitcoin.BitcoinBaseWalletProvider.md#sendsweeptransaction)

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

#### Implementation of

IBitcoinWallet.sendTransaction

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[sendTransaction](chainify_bitcoin.BitcoinBaseWalletProvider.md#sendtransaction)

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:111](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L111)

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

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[setChainProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md#setchainprovider)

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

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[setNamingProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md#setnamingprovider)

#### Defined in

client/dist/lib/Wallet.d.ts:9

___

### signBatchP2SHTransaction

▸ **signBatchP2SHTransaction**(`inputs`, `addresses`, `tx`, `lockTime?`, `segwit?`): `Promise`<`Buffer`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `inputs` | [{ `index`: `number` ; `inputTxHex`: `string` ; `outputScript`: `Buffer` ; `txInputIndex?`: `number` ; `vout`: `any`  }] |
| `addresses` | `string` |
| `tx` | `any` |
| `lockTime?` | `number` |
| `segwit?` | `boolean` |

#### Returns

`Promise`<`Buffer`[]\>

#### Overrides

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[signBatchP2SHTransaction](chainify_bitcoin.BitcoinBaseWalletProvider.md#signbatchp2shtransaction)

#### Defined in

[bitcoin/lib/wallet/BitcoinHDWallet.ts:171](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinHDWallet.ts#L171)

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

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[signMessage](chainify_bitcoin.BitcoinBaseWalletProvider.md#signmessage)

#### Defined in

[bitcoin/lib/wallet/BitcoinHDWallet.ts:45](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinHDWallet.ts#L45)

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

#### Overrides

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[signPSBT](chainify_bitcoin.BitcoinBaseWalletProvider.md#signpsbt)

#### Defined in

[bitcoin/lib/wallet/BitcoinHDWallet.ts:162](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinHDWallet.ts#L162)

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

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[signTypedData](chainify_bitcoin.BitcoinBaseWalletProvider.md#signtypeddata)

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

#### Implementation of

IBitcoinWallet.updateTransactionFee

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[updateTransactionFee](chainify_bitcoin.BitcoinBaseWalletProvider.md#updatetransactionfee)

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

#### Inherited from

[BitcoinBaseWalletProvider](chainify_bitcoin.BitcoinBaseWalletProvider.md).[withCachedUtxos](chainify_bitcoin.BitcoinBaseWalletProvider.md#withcachedutxos)

#### Defined in

[bitcoin/lib/wallet/BitcoinBaseWallet.ts:284](https://github.com/liquality/chainify/blob/540cfa69/packages/bitcoin/lib/wallet/BitcoinBaseWallet.ts#L284)
