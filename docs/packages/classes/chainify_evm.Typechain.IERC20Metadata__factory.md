---
id: "chainify_evm.Typechain.IERC20Metadata__factory"
title: "Class: IERC20Metadata__factory"
sidebar_label: "IERC20Metadata__factory"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).IERC20Metadata__factory

## Constructors

### constructor

• **new IERC20Metadata__factory**()

## Properties

### abi

▪ `Static` `Readonly` **abi**: ({ `anonymous`: `boolean` = false; `inputs`: { `indexed`: `boolean` = true; `internalType`: `string` = "address"; `name`: `string` = "owner"; `type`: `string` = "address" }[] ; `name`: `string` = "Approval"; `outputs`: `undefined` ; `stateMutability`: `undefined` = "view"; `type`: `string` = "event" } \| { `anonymous`: `undefined` = false; `inputs`: { `internalType`: `string` = "address"; `name`: `string` = "owner"; `type`: `string` = "address" }[] ; `name`: `string` = "allowance"; `outputs`: { `internalType`: `string` = "uint256"; `name`: `string` = ""; `type`: `string` = "uint256" }[] ; `stateMutability`: `string` = "view"; `type`: `string` = "function" })[] = `_abi`

#### Defined in

evm/lib/typechain/factories/IERC20Metadata__factory.ts:238

## Methods

### connect

▸ `Static` **connect**(`address`, `signerOrProvider`): [`IERC20Metadata`](../interfaces/chainify_evm.Typechain.IERC20Metadata.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `signerOrProvider` | `Provider` \| `Signer` |

#### Returns

[`IERC20Metadata`](../interfaces/chainify_evm.Typechain.IERC20Metadata.md)

#### Defined in

evm/lib/typechain/factories/IERC20Metadata__factory.ts:242

___

### createInterface

▸ `Static` **createInterface**(): `IERC20MetadataInterface`

#### Returns

`IERC20MetadataInterface`

#### Defined in

evm/lib/typechain/factories/IERC20Metadata__factory.ts:239
