---
id: "chainify_types"
title: "Module: @chainify/types"
sidebar_label: "@chainify/types"
sidebar_position: 0
custom_edit_url: null
---

## Enumerations

- [TxStatus](../enums/chainify_types.TxStatus.md)

## Classes

- [Address](../classes/chainify_types.Address.md)

## Interfaces

- [Asset](../interfaces/chainify_types.Asset.md)
- [Block](../interfaces/chainify_types.Block.md)
- [ChainProvider](../interfaces/chainify_types.ChainProvider.md)
- [EIP1559Fee](../interfaces/chainify_types.EIP1559Fee.md)
- [FeeDetail](../interfaces/chainify_types.FeeDetail.md)
- [FeeDetails](../interfaces/chainify_types.FeeDetails.md)
- [FeeProvider](../interfaces/chainify_types.FeeProvider.md)
- [MultilayerGasPrice](../interfaces/chainify_types.MultilayerGasPrice.md)
- [NFTAsset](../interfaces/chainify_types.NFTAsset.md)
- [NamingProvider](../interfaces/chainify_types.NamingProvider.md)
- [Network](../interfaces/chainify_types.Network.md)
- [SwapParams](../interfaces/chainify_types.SwapParams.md)
- [SwapProvider](../interfaces/chainify_types.SwapProvider.md)
- [TokenDetails](../interfaces/chainify_types.TokenDetails.md)
- [Transaction](../interfaces/chainify_types.Transaction.md)
- [WalletOptions](../interfaces/chainify_types.WalletOptions.md)
- [WalletProvider](../interfaces/chainify_types.WalletProvider.md)

## Type aliases

### AddressType

Ƭ **AddressType**: [`Address`](../classes/chainify_types.Address.md) \| `string`

#### Defined in

[types/lib/Address.ts:19](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Address.ts#L19)

___

### AssetType

Ƭ **AssetType**: ``"native"`` \| ``"erc20"``

#### Defined in

[types/lib/Asset.ts:4](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Asset.ts#L4)

___

### BigNumberish

Ƭ **BigNumberish**: `string` \| `number` \| `EthersBigNumberish` \| `BigNumber`

#### Defined in

[types/lib/index.ts:17](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/index.ts#L17)

___

### FeeType

Ƭ **FeeType**: [`EIP1559Fee`](../interfaces/chainify_types.EIP1559Fee.md) \| `number`

#### Defined in

[types/lib/Fees.ts:15](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Fees.ts#L15)

___

### Nullable

Ƭ **Nullable**<`T`\>: `T` \| ``null``

#### Type parameters

| Name |
| :------ |
| `T` |

#### Defined in

[types/lib/index.ts:19](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/index.ts#L19)

___

### TransactionRequest

Ƭ **TransactionRequest**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `asset?` | [`Asset`](../interfaces/chainify_types.Asset.md) |
| `data?` | `string` |
| `fee?` | [`FeeType`](chainify_types.md#feetype) |
| `feeAsset?` | [`Asset`](../interfaces/chainify_types.Asset.md) |
| `gasLimit?` | `number` |
| `to?` | [`AddressType`](chainify_types.md#addresstype) |
| `value?` | `BigNumber` |

#### Defined in

[types/lib/Transaction.ts:47](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Transaction.ts#L47)
