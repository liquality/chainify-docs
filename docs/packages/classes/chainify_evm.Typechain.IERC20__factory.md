---
id: "chainify_evm.Typechain.IERC20__factory"
title: "Class: IERC20__factory"
sidebar_label: "IERC20__factory"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).IERC20__factory

## Constructors

### constructor

• **new IERC20__factory**()

## Properties

### abi

▪ `Static` `Readonly` **abi**: ({ `anonymous`: `boolean` = false; `inputs`: { `indexed`: `boolean` = true; `internalType`: `string` = "address"; `name`: `string` = "owner"; `type`: `string` = "address" }[] ; `name`: `string` = "Approval"; `outputs`: `undefined` ; `stateMutability`: `undefined` = "view"; `type`: `string` = "event" } \| { `anonymous`: `undefined` = false; `inputs`: { `internalType`: `string` = "address"; `name`: `string` = "owner"; `type`: `string` = "address" }[] ; `name`: `string` = "allowance"; `outputs`: { `internalType`: `string` = "uint256"; `name`: `string` = ""; `type`: `string` = "uint256" }[] ; `stateMutability`: `string` = "view"; `type`: `string` = "function" })[] = `_abi`

#### Defined in

evm/lib/typechain/factories/IERC20__factory.ts:196

## Methods

### connect

▸ `Static` **connect**(`address`, `signerOrProvider`): [`IERC20`](../interfaces/chainify_evm.Typechain.IERC20.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `signerOrProvider` | `Provider` \| `Signer` |

#### Returns

[`IERC20`](../interfaces/chainify_evm.Typechain.IERC20.md)

#### Defined in

evm/lib/typechain/factories/IERC20__factory.ts:200

___

### createInterface

▸ `Static` **createInterface**(): `IERC20Interface`

#### Returns

`IERC20Interface`

#### Defined in

evm/lib/typechain/factories/IERC20__factory.ts:197
