---
id: "chainify_solana.SolanaChainProvider"
title: "Class: SolanaChainProvider"
sidebar_label: "SolanaChainProvider"
custom_edit_url: null
---

[@chainify/solana](../modules/chainify_solana.md).SolanaChainProvider

## Hierarchy

- `default`<`Connection`, `Network`\>

  ↳ **`SolanaChainProvider`**

## Constructors

### constructor

• **new SolanaChainProvider**(`network`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `network` | `Network` |

#### Overrides

Chain&lt;Connection, Network\&gt;.constructor

#### Defined in

[solana/lib/chain/SolanaChainProvider.ts:14](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/chain/SolanaChainProvider.ts#L14)

## Properties

### feeProvider

• `Protected` **feeProvider**: `default`

#### Inherited from

Chain.feeProvider

#### Defined in

client/dist/lib/Chain.d.ts:11

___

### network

• `Protected` **network**: `Network`

#### Inherited from

Chain.network

#### Defined in

client/dist/lib/Chain.d.ts:12

___

### provider

• `Protected` **provider**: `Connection`

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

[solana/lib/chain/SolanaChainProvider.ts:62](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/chain/SolanaChainProvider.ts#L62)

___

### getBlockByHash

▸ **getBlockByHash**(`_blockHash`): `Promise`<`Block`<`Block`<`any`, `any`\>, `Transaction`<`any`\>\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_blockHash` | `string` |

#### Returns

`Promise`<`Block`<`Block`<`any`, `any`\>, `Transaction`<`any`\>\>\>

#### Overrides

Chain.getBlockByHash

#### Defined in

[solana/lib/chain/SolanaChainProvider.ts:118](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/chain/SolanaChainProvider.ts#L118)

___

### getBlockByNumber

▸ **getBlockByNumber**(`blockNumber?`, `includeTx?`): `Promise`<`Block`<`BlockResponse`, `Transaction`<`any`\>\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `blockNumber?` | `number` |
| `includeTx?` | `boolean` |

#### Returns

`Promise`<`Block`<`BlockResponse`, `Transaction`<`any`\>\>\>

#### Overrides

Chain.getBlockByNumber

#### Defined in

[solana/lib/chain/SolanaChainProvider.ts:22](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/chain/SolanaChainProvider.ts#L22)

___

### getBlockHeight

▸ **getBlockHeight**(): `Promise`<`number`\>

#### Returns

`Promise`<`number`\>

#### Overrides

Chain.getBlockHeight

#### Defined in

[solana/lib/chain/SolanaChainProvider.ts:43](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/chain/SolanaChainProvider.ts#L43)

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

▸ **getFees**(): `Promise`<`FeeDetails`\>

#### Returns

`Promise`<`FeeDetails`\>

#### Overrides

Chain.getFees

#### Defined in

[solana/lib/chain/SolanaChainProvider.ts:95](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/chain/SolanaChainProvider.ts#L95)

___

### getNetwork

▸ **getNetwork**(): `Network`

#### Returns

`Network`

#### Inherited from

Chain.getNetwork

#### Defined in

client/dist/lib/Chain.d.ts:22

___

### getProvider

▸ **getProvider**(): `Connection`

#### Returns

`Connection`

#### Inherited from

Chain.getProvider

#### Defined in

client/dist/lib/Chain.d.ts:26

___

### getTokenDetails

▸ **getTokenDetails**(`_asset`): `Promise`<`TokenDetails`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_asset` | `string` |

#### Returns

`Promise`<`TokenDetails`\>

#### Inherited from

Chain.getTokenDetails

#### Defined in

client/dist/lib/Chain.d.ts:42

___

### getTransactionByHash

▸ **getTransactionByHash**(`txHash`): `Promise`<`Transaction`<`any`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `txHash` | `string` |

#### Returns

`Promise`<`Transaction`<`any`\>\>

#### Overrides

Chain.getTransactionByHash

#### Defined in

[solana/lib/chain/SolanaChainProvider.ts:47](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/chain/SolanaChainProvider.ts#L47)

___

### sendRawTransaction

▸ **sendRawTransaction**(`rawTransaction`): `Promise`<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `rawTransaction` | `string` |

#### Returns

`Promise`<`string`\>

#### Overrides

Chain.sendRawTransaction

#### Defined in

[solana/lib/chain/SolanaChainProvider.ts:109](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/chain/SolanaChainProvider.ts#L109)

___

### sendRpcRequest

▸ **sendRpcRequest**(`_method`, `_params`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `_method` | `string` |
| `_params` | `any`[] |

#### Returns

`Promise`<`void`\>

#### Overrides

Chain.sendRpcRequest

#### Defined in

[solana/lib/chain/SolanaChainProvider.ts:114](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/chain/SolanaChainProvider.ts#L114)

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
| `network` | `Network` |

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
| `provider` | `Connection` |

#### Returns

`Promise`<`void`\>

#### Inherited from

Chain.setProvider

#### Defined in

client/dist/lib/Chain.d.ts:30
