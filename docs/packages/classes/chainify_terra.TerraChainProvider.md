---
id: "chainify_terra.TerraChainProvider"
title: "Class: TerraChainProvider"
sidebar_label: "TerraChainProvider"
custom_edit_url: null
---

[@chainify/terra](../modules/chainify_terra.md).TerraChainProvider

## Hierarchy

- `default`<`LCDClient`, [`TerraNetwork`](../interfaces/chainify_terra.TerraTypes.TerraNetwork.md)\>

  ↳ **`TerraChainProvider`**

## Constructors

### constructor

• **new TerraChainProvider**(`network`, `provider?`, `feeProvider?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `network` | [`TerraNetwork`](../interfaces/chainify_terra.TerraTypes.TerraNetwork.md) |
| `provider?` | `LCDClient` |
| `feeProvider?` | `default` |

#### Overrides

Chain&lt;LCDClient, TerraNetwork\&gt;.constructor

#### Defined in

[terra/lib/chain/TerraChainProvider.ts:17](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/chain/TerraChainProvider.ts#L17)

## Properties

### \_httpClient

• **\_httpClient**: `default`

#### Defined in

[terra/lib/chain/TerraChainProvider.ts:15](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/chain/TerraChainProvider.ts#L15)

___

### feeProvider

• `Protected` **feeProvider**: `default`

#### Inherited from

Chain.feeProvider

#### Defined in

client/dist/lib/Chain.d.ts:11

___

### network

• `Protected` **network**: [`TerraNetwork`](../interfaces/chainify_terra.TerraTypes.TerraNetwork.md)

#### Inherited from

Chain.network

#### Defined in

client/dist/lib/Chain.d.ts:12

___

### provider

• `Protected` **provider**: `LCDClient`

#### Inherited from

Chain.provider

#### Defined in

client/dist/lib/Chain.d.ts:13

## Methods

### getBalance

▸ **getBalance**(`addresses`, `assets`): `Promise`<`BigNumber`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `addresses` | `AddressType`[] |
| `assets` | `Asset`[] |

#### Returns

`Promise`<`BigNumber`[]\>

#### Overrides

Chain.getBalance

#### Defined in

[terra/lib/chain/TerraChainProvider.ts:70](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/chain/TerraChainProvider.ts#L70)

___

### getBlockByHash

▸ **getBlockByHash**(`_blockHash`, `_includeTx?`): `Promise`<`Block`<`BlockInfo`, [`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_blockHash` | `string` |
| `_includeTx?` | `boolean` |

#### Returns

`Promise`<`Block`<`BlockInfo`, [`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Overrides

Chain.getBlockByHash

#### Defined in

[terra/lib/chain/TerraChainProvider.ts:122](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/chain/TerraChainProvider.ts#L122)

___

### getBlockByNumber

▸ **getBlockByNumber**(`blockNumber?`, `includeTx?`): `Promise`<`Block`<`BlockInfo`, [`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `blockNumber?` | `number` |
| `includeTx?` | `boolean` |

#### Returns

`Promise`<`Block`<`BlockInfo`, [`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Overrides

Chain.getBlockByNumber

#### Defined in

[terra/lib/chain/TerraChainProvider.ts:41](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/chain/TerraChainProvider.ts#L41)

___

### getBlockHeight

▸ **getBlockHeight**(): `Promise`<`number`\>

#### Returns

`Promise`<`number`\>

#### Overrides

Chain.getBlockHeight

#### Defined in

[terra/lib/chain/TerraChainProvider.ts:54](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/chain/TerraChainProvider.ts#L54)

___

### getFeeProvider

▸ **getFeeProvider**(): `Promise`<`default`\>

#### Returns

`Promise`<`default`\>

#### Inherited from

Chain.getFeeProvider

#### Defined in

client/dist/lib/Chain.d.ts:38

___

### getFees

▸ **getFees**(`feeAsset?`): `Promise`<`FeeDetails`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `feeAsset?` | `Asset` |

#### Returns

`Promise`<`FeeDetails`\>

#### Overrides

Chain.getFees

#### Defined in

[terra/lib/chain/TerraChainProvider.ts:102](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/chain/TerraChainProvider.ts#L102)

___

### getNetwork

▸ **getNetwork**(): [`TerraNetwork`](../interfaces/chainify_terra.TerraTypes.TerraNetwork.md)

#### Returns

[`TerraNetwork`](../interfaces/chainify_terra.TerraTypes.TerraNetwork.md)

#### Inherited from

Chain.getNetwork

#### Defined in

client/dist/lib/Chain.d.ts:22

___

### getProvider

▸ **getProvider**(): `LCDClient`

#### Returns

`LCDClient`

#### Inherited from

Chain.getProvider

#### Defined in

client/dist/lib/Chain.d.ts:26

___

### getTokenDetails

▸ **getTokenDetails**(`asset`): `Promise`<`TokenDetails`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `asset` | `string` |

#### Returns

`Promise`<`TokenDetails`\>

#### Overrides

Chain.getTokenDetails

#### Defined in

[terra/lib/chain/TerraChainProvider.ts:27](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/chain/TerraChainProvider.ts#L27)

___

### getTransactionByHash

▸ **getTransactionByHash**(`txHash`): `Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txHash` | `string` |

#### Returns

`Promise`<`Transaction`<[`TerraTxInfo`](../interfaces/chainify_terra.TerraTypes.TerraTxInfo.md)\>\>

#### Overrides

Chain.getTransactionByHash

#### Defined in

[terra/lib/chain/TerraChainProvider.ts:59](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/chain/TerraChainProvider.ts#L59)

___

### sendRawTransaction

▸ **sendRawTransaction**(`_rawTransaction`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_rawTransaction` | `string` |

#### Returns

`Promise`<`string`\>

#### Overrides

Chain.sendRawTransaction

#### Defined in

[terra/lib/chain/TerraChainProvider.ts:126](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/chain/TerraChainProvider.ts#L126)

___

### sendRpcRequest

▸ **sendRpcRequest**(`method`, `params`): `Promise`<`any`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `method` | keyof `APIRequester` |
| `params` | `any`[] |

#### Returns

`Promise`<`any`\>

#### Overrides

Chain.sendRpcRequest

#### Defined in

[terra/lib/chain/TerraChainProvider.ts:117](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/chain/TerraChainProvider.ts#L117)

___

### setFeeProvider

▸ **setFeeProvider**(`feeProvider`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `feeProvider` | `default` |

#### Returns

`Promise`<`void`\>

#### Inherited from

Chain.setFeeProvider

#### Defined in

client/dist/lib/Chain.d.ts:34

___

### setNetwork

▸ **setNetwork**(`network`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `network` | [`TerraNetwork`](../interfaces/chainify_terra.TerraTypes.TerraNetwork.md) |

#### Returns

`void`

#### Inherited from

Chain.setNetwork

#### Defined in

client/dist/lib/Chain.d.ts:18

___

### setProvider

▸ **setProvider**(`provider`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `provider` | `LCDClient` |

#### Returns

`Promise`<`void`\>

#### Inherited from

Chain.setProvider

#### Defined in

client/dist/lib/Chain.d.ts:30
