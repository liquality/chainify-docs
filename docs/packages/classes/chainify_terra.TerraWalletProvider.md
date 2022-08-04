---
id: "chainify_terra.TerraWalletProvider"
title: "Class: TerraWalletProvider"
sidebar_label: "TerraWalletProvider"
custom_edit_url: null
---

[@chainify/terra](../modules/chainify_terra.md).TerraWalletProvider

## Hierarchy

- `default`<`LCDClient`, `MnemonicKey`\>

  ↳ **`TerraWalletProvider`**

## Constructors

### constructor

• **new TerraWalletProvider**(`walletOptions`, `chainProvider?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `walletOptions` | [`TerraWalletProviderOptions`](../interfaces/chainify_terra.TerraTypes.TerraWalletProviderOptions.md) |
| `chainProvider?` | [`TerraChainProvider`](chainify_terra.TerraChainProvider.md) |

#### Overrides

Wallet&lt;LCDClient, MnemonicKey\&gt;.constructor

#### Defined in

[terra/lib/wallet/TerraWalletProvider.ts:32](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L32)

## Properties

### chainProvider

• `Protected` **chainProvider**: `default`<`LCDClient`, `Network`\>

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

• `Protected` **signer**: `MnemonicKey`

#### Defined in

[terra/lib/wallet/TerraWalletProvider.ts:24](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L24)

## Methods

### canUpdateFee

▸ **canUpdateFee**(): `boolean`

#### Returns

`boolean`

#### Overrides

Wallet.canUpdateFee

#### Defined in

[terra/lib/wallet/TerraWalletProvider.ts:133](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L133)

___

### exportPrivateKey

▸ **exportPrivateKey**(): `Promise`<`string`\>

#### Returns

`Promise`<`string`\>

#### Overrides

Wallet.exportPrivateKey

#### Defined in

[terra/lib/wallet/TerraWalletProvider.ts:46](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L46)

___

### getAddress

▸ **getAddress**(): `Promise`<`Address`\>

#### Returns

`Promise`<`Address`\>

#### Overrides

Wallet.getAddress

#### Defined in

[terra/lib/wallet/TerraWalletProvider.ts:55](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L55)

___

### getAddresses

▸ **getAddresses**(): `Promise`<`Address`[]\>

#### Returns

`Promise`<`Address`[]\>

#### Overrides

Wallet.getAddresses

#### Defined in

[terra/lib/wallet/TerraWalletProvider.ts:72](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L72)

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

[terra/lib/wallet/TerraWalletProvider.ts:128](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L128)

___

### getChainProvider

▸ **getChainProvider**(): `default`<`LCDClient`, `Network`\>

#### Returns

`default`<`LCDClient`, `Network`\>

#### Inherited from

Wallet.getChainProvider

#### Defined in

client/dist/lib/Wallet.d.ts:8

___

### getConnectedNetwork

▸ **getConnectedNetwork**(): `Promise`<[`TerraNetwork`](../interfaces/chainify_terra.TerraTypes.TerraNetwork.md)\>

#### Returns

`Promise`<[`TerraNetwork`](../interfaces/chainify_terra.TerraTypes.TerraNetwork.md)\>

#### Overrides

Wallet.getConnectedNetwork

#### Defined in

[terra/lib/wallet/TerraWalletProvider.ts:91](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L91)

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

▸ **getSigner**(): `MnemonicKey`

#### Returns

`MnemonicKey`

#### Overrides

Wallet.getSigner

#### Defined in

[terra/lib/wallet/TerraWalletProvider.ts:115](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L115)

___

### getUnusedAddress

▸ **getUnusedAddress**(): `Promise`<`Address`\>

#### Returns

`Promise`<`Address`\>

#### Overrides

Wallet.getUnusedAddress

#### Defined in

[terra/lib/wallet/TerraWalletProvider.ts:81](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L81)

___

### getUsedAddresses

▸ **getUsedAddresses**(): `Promise`<`Address`[]\>

#### Returns

`Promise`<`Address`[]\>

#### Overrides

Wallet.getUsedAddresses

#### Defined in

[terra/lib/wallet/TerraWalletProvider.ts:77](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L77)

___

### isWalletAvailable

▸ **isWalletAvailable**(): `Promise`<`boolean`\>

#### Returns

`Promise`<`boolean`\>

#### Overrides

Wallet.isWalletAvailable

#### Defined in

[terra/lib/wallet/TerraWalletProvider.ts:50](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L50)

___

### onChainProviderUpdate

▸ `Protected` **onChainProviderUpdate**(`chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider` | [`TerraChainProvider`](chainify_terra.TerraChainProvider.md) |

#### Returns

`void`

#### Overrides

Wallet.onChainProviderUpdate

#### Defined in

[terra/lib/wallet/TerraWalletProvider.ts:137](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L137)

___

### sendBatchTransaction

▸ **sendBatchTransaction**(`_txRequests`): `Promise`<`Transaction`<`any`\>[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_txRequests` | `TransactionRequest`[] |

#### Returns

`Promise`<`Transaction`<`any`\>[]\>

#### Overrides

Wallet.sendBatchTransaction

#### Defined in

[terra/lib/wallet/TerraWalletProvider.ts:120](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L120)

___

### sendSweepTransaction

▸ **sendSweepTransaction**(`address`, `asset`): `Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` \| `Address` |
| `asset` | `Asset` |

#### Returns

`Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Overrides

Wallet.sendSweepTransaction

#### Defined in

[terra/lib/wallet/TerraWalletProvider.ts:109](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L109)

___

### sendTransaction

▸ **sendTransaction**(`txRequest`): `Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txRequest` | [`TerraTxRequest`](../interfaces/chainify_terra.TerraTypes.TerraTxRequest.md) |

#### Returns

`Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Overrides

Wallet.sendTransaction

#### Defined in

[terra/lib/wallet/TerraWalletProvider.ts:95](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L95)

___

### setChainProvider

▸ **setChainProvider**(`chainProvider`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chainProvider` | `default`<`LCDClient`, `Network`\> |

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

[terra/lib/wallet/TerraWalletProvider.ts:86](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L86)

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

[terra/lib/wallet/TerraWalletProvider.ts:124](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/wallet/TerraWalletProvider.ts#L124)
