---
id: "chainify_evm.Typechain.IERC165__factory"
title: "Class: IERC165__factory"
sidebar_label: "IERC165__factory"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).IERC165__factory

## Constructors

### constructor

• **new IERC165__factory**()

## Properties

### abi

▪ `Static` `Readonly` **abi**: { `inputs`: { `internalType`: `string` = "bytes4"; `name`: `string` = "interfaceId"; `type`: `string` = "bytes4" }[] ; `name`: `string` = "supportsInterface"; `outputs`: { `internalType`: `string` = "bool"; `name`: `string` = ""; `type`: `string` = "bool" }[] ; `stateMutability`: `string` = "view"; `type`: `string` = "function" }[] = `_abi`

#### Defined in

evm/lib/typechain/factories/IERC165__factory.ts:32

## Methods

### connect

▸ `Static` **connect**(`address`, `signerOrProvider`): [`IERC165`](../interfaces/chainify_evm.Typechain.IERC165.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `signerOrProvider` | `Provider` \| `Signer` |

#### Returns

[`IERC165`](../interfaces/chainify_evm.Typechain.IERC165.md)

#### Defined in

evm/lib/typechain/factories/IERC165__factory.ts:36

___

### createInterface

▸ `Static` **createInterface**(): `IERC165Interface`

#### Returns

`IERC165Interface`

#### Defined in

evm/lib/typechain/factories/IERC165__factory.ts:33
