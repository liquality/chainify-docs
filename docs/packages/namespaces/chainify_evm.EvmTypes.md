---
id: "chainify_evm.EvmTypes"
title: "Namespace: EvmTypes"
sidebar_label: "EvmTypes"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).EvmTypes

## Enumerations

- [NftTypes](../enums/chainify_evm.EvmTypes.NftTypes.md)

## Interfaces

- [EvmSwapOptions](../interfaces/chainify_evm.EvmTypes.EvmSwapOptions.md)
- [MulticallData](../interfaces/chainify_evm.EvmTypes.MulticallData.md)
- [SignTypedMessageType](../interfaces/chainify_evm.EvmTypes.SignTypedMessageType.md)

## Type aliases

### EthereumFeeData

Ƭ **EthereumFeeData**: `FeeType` & { `gasPrice?`: ``null`` \| `number` ; `maxFeePerGas?`: ``null`` \| `number` ; `maxPriorityFeePerGas?`: ``null`` \| `number`  }

#### Defined in

[evm/lib/types.ts:38](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/types.ts#L38)

___

### EthereumTransactionRequest

Ƭ **EthereumTransactionRequest**: `TransactionRequest` & { `chainId?`: `number` ; `from?`: `AddressType` ; `gasLimit?`: `number` ; `gasPrice?`: `number` ; `maxFeePerGas?`: `number` ; `maxPriorityFeePerGas?`: `number` ; `nonce?`: `number` ; `type?`: `number`  }

#### Defined in

[evm/lib/types.ts:27](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/types.ts#L27)

___

### FeeOptions

Ƭ **FeeOptions**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `averageMultiplier?` | `number` |
| `fastMultiplier?` | `number` |
| `slowMultiplier?` | `number` |

#### Defined in

[evm/lib/types.ts:21](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/types.ts#L21)

___

### MoralisConfig

Ƭ **MoralisConfig**: [`NftProviderConfig`](chainify_evm.EvmTypes.md#nftproviderconfig) & { `appId`: `string`  }

#### Defined in

[evm/lib/types.ts:56](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/types.ts#L56)

___

### NftProviderConfig

Ƭ **NftProviderConfig**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `apiKey` | `string` |
| `url` | `string` |

#### Defined in

[evm/lib/types.ts:51](https://github.com/liquality/chainify/blob/540cfa69/packages/evm/lib/types.ts#L51)
