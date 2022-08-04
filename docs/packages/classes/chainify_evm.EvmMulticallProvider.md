---
id: "chainify_evm.EvmMulticallProvider"
title: "Class: EvmMulticallProvider"
sidebar_label: "EvmMulticallProvider"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).EvmMulticallProvider

## Constructors

### constructor

• **new EvmMulticallProvider**(`chainProvider`, `multicallAddress?`)

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `chainProvider` | `BaseProvider` | `undefined` |
| `multicallAddress` | `string` | `'0xcA11bde05977b3631167028862bE2a173976CA11'` |

#### Defined in

[evm/lib/chain/EvmMulticallProvider.ts:17](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmMulticallProvider.ts#L17)

## Methods

### buildBalanceCallData

▸ **buildBalanceCallData**(`asset`, `user`): { `abi`: { `inputs`: ({ `components`: `undefined` ; `internalType`: `string` = "bool"; `name`: `string` = "requireSuccess"; `type`: `string` = "bool" } \| { `components`: { `internalType`: `string` = "address"; `name`: `string` = "target"; `type`: `string` = "address" }[] ; `internalType`: `string` = "struct Multicall3.Call[]"; `name`: `string` = "calls"; `type`: `string` = "tuple[]" })[] ; `name`: `string` = "tryBlockAndAggregate"; `outputs`: ({ `components`: `undefined` ; `internalType`: `string` = "uint256"; `name`: `string` = "blockNumber"; `type`: `string` = "uint256" } \| { `components`: { `internalType`: `string` = "bool"; `name`: `string` = "success"; `type`: `string` = "bool" }[] ; `internalType`: `string` = "struct Multicall3.Result[]"; `name`: `string` = "returnData"; `type`: `string` = "tuple[]" })[] ; `stateMutability`: `string` = "payable"; `type`: `string` = "function" }[] = Multicall3\_\_factory.abi; `name`: `string` = 'getEthBalance'; `params`: `AddressType`[] ; `target`: `string`  } \| { `abi`: ({ `anonymous`: `undefined` = false; `inputs`: { `internalType`: `string` = "string"; `name`: `string` = "name\_"; `type`: `string` = "string" }[] ; `name`: `undefined` = "allowance"; `outputs`: `undefined` ; `stateMutability`: `string` = "nonpayable"; `type`: `string` = "constructor" } \| { `anonymous`: `boolean` = false; `inputs`: { `indexed`: `boolean` = true; `internalType`: `string` = "address"; `name`: `string` = "owner"; `type`: `string` = "address" }[] ; `name`: `string` = "Approval"; `outputs`: `undefined` ; `stateMutability`: `undefined` = "view"; `type`: `string` = "event" } \| { `anonymous`: `undefined` = false; `inputs`: { `internalType`: `string` = "address"; `name`: `string` = "owner"; `type`: `string` = "address" }[] ; `name`: `string` = "allowance"; `outputs`: { `internalType`: `string` = "uint256"; `name`: `string` = ""; `type`: `string` = "uint256" }[] ; `stateMutability`: `string` = "view"; `type`: `string` = "function" })[] = ERC20\_\_factory.abi; `name`: `string` = 'balanceOf'; `params`: `AddressType`[] ; `target`: `string` = asset.contractAddress }

#### Parameters

| Name | Type |
| :------ | :------ |
| `asset` | `Asset` |
| `user` | `AddressType` |

#### Returns

{ `abi`: { `inputs`: ({ `components`: `undefined` ; `internalType`: `string` = "bool"; `name`: `string` = "requireSuccess"; `type`: `string` = "bool" } \| { `components`: { `internalType`: `string` = "address"; `name`: `string` = "target"; `type`: `string` = "address" }[] ; `internalType`: `string` = "struct Multicall3.Call[]"; `name`: `string` = "calls"; `type`: `string` = "tuple[]" })[] ; `name`: `string` = "tryBlockAndAggregate"; `outputs`: ({ `components`: `undefined` ; `internalType`: `string` = "uint256"; `name`: `string` = "blockNumber"; `type`: `string` = "uint256" } \| { `components`: { `internalType`: `string` = "bool"; `name`: `string` = "success"; `type`: `string` = "bool" }[] ; `internalType`: `string` = "struct Multicall3.Result[]"; `name`: `string` = "returnData"; `type`: `string` = "tuple[]" })[] ; `stateMutability`: `string` = "payable"; `type`: `string` = "function" }[] = Multicall3\_\_factory.abi; `name`: `string` = 'getEthBalance'; `params`: `AddressType`[] ; `target`: `string`  } \| { `abi`: ({ `anonymous`: `undefined` = false; `inputs`: { `internalType`: `string` = "string"; `name`: `string` = "name\_"; `type`: `string` = "string" }[] ; `name`: `undefined` = "allowance"; `outputs`: `undefined` ; `stateMutability`: `string` = "nonpayable"; `type`: `string` = "constructor" } \| { `anonymous`: `boolean` = false; `inputs`: { `indexed`: `boolean` = true; `internalType`: `string` = "address"; `name`: `string` = "owner"; `type`: `string` = "address" }[] ; `name`: `string` = "Approval"; `outputs`: `undefined` ; `stateMutability`: `undefined` = "view"; `type`: `string` = "event" } \| { `anonymous`: `undefined` = false; `inputs`: { `internalType`: `string` = "address"; `name`: `string` = "owner"; `type`: `string` = "address" }[] ; `name`: `string` = "allowance"; `outputs`: { `internalType`: `string` = "uint256"; `name`: `string` = ""; `type`: `string` = "uint256" }[] ; `stateMutability`: `string` = "view"; `type`: `string` = "function" })[] = ERC20\_\_factory.abi; `name`: `string` = 'balanceOf'; `params`: `AddressType`[] ; `target`: `string` = asset.contractAddress }

#### Defined in

[evm/lib/chain/EvmMulticallProvider.ts:26](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmMulticallProvider.ts#L26)

___

### getEthBalance

▸ **getEthBalance**(`address`): `Promise`<`BigNumber`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |

#### Returns

`Promise`<`BigNumber`\>

#### Defined in

[evm/lib/chain/EvmMulticallProvider.ts:49](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmMulticallProvider.ts#L49)

___

### getMulticallAddress

▸ **getMulticallAddress**(): `string`

#### Returns

`string`

#### Defined in

[evm/lib/chain/EvmMulticallProvider.ts:22](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmMulticallProvider.ts#L22)

___

### getMultipleBalances

▸ **getMultipleBalances**(`address`, `assets`): `Promise`<`BigNumber`[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `AddressType` |
| `assets` | `Asset`[] |

#### Returns

`Promise`<`BigNumber`[]\>

#### Defined in

[evm/lib/chain/EvmMulticallProvider.ts:53](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmMulticallProvider.ts#L53)

___

### multicall

▸ **multicall**<`T`\>(`calls`): `Promise`<`T`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `any`[] = `any`[] |

#### Parameters

| Name | Type |
| :------ | :------ |
| `calls` | readonly [`MulticallData`](../interfaces/chainify_evm.EvmTypes.MulticallData.md)[] |

#### Returns

`Promise`<`T`\>

#### Defined in

[evm/lib/chain/EvmMulticallProvider.ts:59](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmMulticallProvider.ts#L59)

___

### setMulticallAddress

▸ **setMulticallAddress**(`multicallAddress`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `multicallAddress` | `string` |

#### Returns

`void`

#### Defined in

[evm/lib/chain/EvmMulticallProvider.ts:44](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/chain/EvmMulticallProvider.ts#L44)
