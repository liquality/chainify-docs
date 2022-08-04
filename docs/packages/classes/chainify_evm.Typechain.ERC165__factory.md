---
id: "chainify_evm.Typechain.ERC165__factory"
title: "Class: ERC165__factory"
sidebar_label: "ERC165__factory"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).ERC165__factory

## Constructors

### constructor

• **new ERC165__factory**()

## Properties

### abi

▪ `Static` `Readonly` **abi**: { `inputs`: { `internalType`: `string` = "bytes4"; `name`: `string` = "interfaceId"; `type`: `string` = "bytes4" }[] ; `name`: `string` = "supportsInterface"; `outputs`: { `internalType`: `string` = "bool"; `name`: `string` = ""; `type`: `string` = "bool" }[] ; `stateMutability`: `string` = "view"; `type`: `string` = "function" }[] = `_abi`

#### Defined in

evm/lib/typechain/factories/ERC165__factory.ts:32

## Methods

### connect

▸ `Static` **connect**(`address`, `signerOrProvider`): [`ERC165`](../interfaces/chainify_evm.Typechain.ERC165.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `signerOrProvider` | `Provider` \| `Signer` |

#### Returns

[`ERC165`](../interfaces/chainify_evm.Typechain.ERC165.md)

#### Defined in

evm/lib/typechain/factories/ERC165__factory.ts:36

___

### createInterface

▸ `Static` **createInterface**(): `ERC165Interface`

#### Returns

`ERC165Interface`

#### Defined in

evm/lib/typechain/factories/ERC165__factory.ts:33
