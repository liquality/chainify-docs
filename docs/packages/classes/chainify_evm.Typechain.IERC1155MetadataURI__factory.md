---
id: "chainify_evm.Typechain.IERC1155MetadataURI__factory"
title: "Class: IERC1155MetadataURI__factory"
sidebar_label: "IERC1155MetadataURI__factory"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).IERC1155MetadataURI__factory

## Constructors

### constructor

• **new IERC1155MetadataURI__factory**()

## Properties

### abi

▪ `Static` `Readonly` **abi**: ({ `anonymous`: `boolean` = false; `inputs`: { `indexed`: `boolean` = true; `internalType`: `string` = "address"; `name`: `string` = "account"; `type`: `string` = "address" }[] ; `name`: `string` = "ApprovalForAll"; `outputs`: `undefined` ; `stateMutability`: `undefined` = "view"; `type`: `string` = "event" } \| { `anonymous`: `undefined` = false; `inputs`: { `internalType`: `string` = "address"; `name`: `string` = "account"; `type`: `string` = "address" }[] ; `name`: `string` = "balanceOf"; `outputs`: { `internalType`: `string` = "uint256"; `name`: `string` = ""; `type`: `string` = "uint256" }[] ; `stateMutability`: `string` = "view"; `type`: `string` = "function" })[] = `_abi`

#### Defined in

evm/lib/typechain/factories/IERC1155MetadataURI__factory.ts:328

## Methods

### connect

▸ `Static` **connect**(`address`, `signerOrProvider`): [`IERC1155MetadataURI`](../interfaces/chainify_evm.Typechain.IERC1155MetadataURI.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `signerOrProvider` | `Provider` \| `Signer` |

#### Returns

[`IERC1155MetadataURI`](../interfaces/chainify_evm.Typechain.IERC1155MetadataURI.md)

#### Defined in

evm/lib/typechain/factories/IERC1155MetadataURI__factory.ts:332

___

### createInterface

▸ `Static` **createInterface**(): `IERC1155MetadataURIInterface`

#### Returns

`IERC1155MetadataURIInterface`

#### Defined in

evm/lib/typechain/factories/IERC1155MetadataURI__factory.ts:329
