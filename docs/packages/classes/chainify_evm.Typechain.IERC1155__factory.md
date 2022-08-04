---
id: "chainify_evm.Typechain.IERC1155__factory"
title: "Class: IERC1155__factory"
sidebar_label: "IERC1155__factory"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).IERC1155__factory

## Constructors

### constructor

• **new IERC1155__factory**()

## Properties

### abi

▪ `Static` `Readonly` **abi**: ({ `anonymous`: `boolean` = false; `inputs`: { `indexed`: `boolean` = true; `internalType`: `string` = "address"; `name`: `string` = "account"; `type`: `string` = "address" }[] ; `name`: `string` = "ApprovalForAll"; `outputs`: `undefined` ; `stateMutability`: `undefined` = "view"; `type`: `string` = "event" } \| { `anonymous`: `undefined` = false; `inputs`: { `internalType`: `string` = "address"; `name`: `string` = "account"; `type`: `string` = "address" }[] ; `name`: `string` = "balanceOf"; `outputs`: { `internalType`: `string` = "uint256"; `name`: `string` = ""; `type`: `string` = "uint256" }[] ; `stateMutability`: `string` = "view"; `type`: `string` = "function" })[] = `_abi`

#### Defined in

evm/lib/typechain/factories/IERC1155__factory.ts:306

## Methods

### connect

▸ `Static` **connect**(`address`, `signerOrProvider`): [`IERC1155`](../interfaces/chainify_evm.Typechain.IERC1155.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `signerOrProvider` | `Provider` \| `Signer` |

#### Returns

[`IERC1155`](../interfaces/chainify_evm.Typechain.IERC1155.md)

#### Defined in

evm/lib/typechain/factories/IERC1155__factory.ts:310

___

### createInterface

▸ `Static` **createInterface**(): `IERC1155Interface`

#### Returns

`IERC1155Interface`

#### Defined in

evm/lib/typechain/factories/IERC1155__factory.ts:307
