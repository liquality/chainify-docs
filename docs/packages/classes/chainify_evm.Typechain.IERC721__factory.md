---
id: "chainify_evm.Typechain.IERC721__factory"
title: "Class: IERC721__factory"
sidebar_label: "IERC721__factory"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).IERC721__factory

## Constructors

### constructor

• **new IERC721__factory**()

## Properties

### abi

▪ `Static` `Readonly` **abi**: ({ `anonymous`: `boolean` = false; `inputs`: { `indexed`: `boolean` = true; `internalType`: `string` = "address"; `name`: `string` = "owner"; `type`: `string` = "address" }[] ; `name`: `string` = "Approval"; `outputs`: `undefined` ; `stateMutability`: `undefined` = "view"; `type`: `string` = "event" } \| { `anonymous`: `undefined` = false; `inputs`: { `internalType`: `string` = "address"; `name`: `string` = "owner"; `type`: `string` = "address" }[] ; `name`: `string` = "balanceOf"; `outputs`: { `internalType`: `string` = "uint256"; `name`: `string` = "balance"; `type`: `string` = "uint256" }[] ; `stateMutability`: `string` = "view"; `type`: `string` = "function" })[] = `_abi`

#### Defined in

evm/lib/typechain/factories/IERC721__factory.ts:298

## Methods

### connect

▸ `Static` **connect**(`address`, `signerOrProvider`): [`IERC721`](../interfaces/chainify_evm.Typechain.IERC721.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `signerOrProvider` | `Provider` \| `Signer` |

#### Returns

[`IERC721`](../interfaces/chainify_evm.Typechain.IERC721.md)

#### Defined in

evm/lib/typechain/factories/IERC721__factory.ts:302

___

### createInterface

▸ `Static` **createInterface**(): `IERC721Interface`

#### Returns

`IERC721Interface`

#### Defined in

evm/lib/typechain/factories/IERC721__factory.ts:299
