---
id: "chainify_evm.Typechain.IERC721Metadata__factory"
title: "Class: IERC721Metadata__factory"
sidebar_label: "IERC721Metadata__factory"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).IERC721Metadata__factory

## Constructors

### constructor

• **new IERC721Metadata__factory**()

## Properties

### abi

▪ `Static` `Readonly` **abi**: ({ `anonymous`: `boolean` = false; `inputs`: { `indexed`: `boolean` = true; `internalType`: `string` = "address"; `name`: `string` = "owner"; `type`: `string` = "address" }[] ; `name`: `string` = "Approval"; `outputs`: `undefined` ; `stateMutability`: `undefined` = "view"; `type`: `string` = "event" } \| { `anonymous`: `undefined` = false; `inputs`: { `internalType`: `string` = "address"; `name`: `string` = "owner"; `type`: `string` = "address" }[] ; `name`: `string` = "balanceOf"; `outputs`: { `internalType`: `string` = "uint256"; `name`: `string` = "balance"; `type`: `string` = "uint256" }[] ; `stateMutability`: `string` = "view"; `type`: `string` = "function" })[] = `_abi`

#### Defined in

evm/lib/typechain/factories/IERC721Metadata__factory.ts:346

## Methods

### connect

▸ `Static` **connect**(`address`, `signerOrProvider`): [`IERC721Metadata`](../interfaces/chainify_evm.Typechain.IERC721Metadata.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `signerOrProvider` | `Provider` \| `Signer` |

#### Returns

[`IERC721Metadata`](../interfaces/chainify_evm.Typechain.IERC721Metadata.md)

#### Defined in

evm/lib/typechain/factories/IERC721Metadata__factory.ts:350

___

### createInterface

▸ `Static` **createInterface**(): `IERC721MetadataInterface`

#### Returns

`IERC721MetadataInterface`

#### Defined in

evm/lib/typechain/factories/IERC721Metadata__factory.ts:347
