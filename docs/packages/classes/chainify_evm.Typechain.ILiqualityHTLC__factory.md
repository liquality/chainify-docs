---
id: "chainify_evm.Typechain.ILiqualityHTLC__factory"
title: "Class: ILiqualityHTLC__factory"
sidebar_label: "ILiqualityHTLC__factory"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).ILiqualityHTLC__factory

## Constructors

### constructor

• **new ILiqualityHTLC__factory**()

## Properties

### abi

▪ `Static` `Readonly` **abi**: ({ `anonymous`: `undefined` = false; `inputs`: `any`[] = []; `name`: `string` = "LiqualityHTLC\_\_InvalidExpiration"; `outputs`: `undefined` ; `stateMutability`: `undefined` = "view"; `type`: `string` = "error" } \| { `anonymous`: `boolean` = false; `inputs`: ({ `components`: `undefined` ; `indexed`: `boolean` = false; `internalType`: `string` = "bytes32"; `name`: `string` = "id"; `type`: `string` = "bytes32" } \| { `components`: { `internalType`: `string` = "uint256"; `name`: `string` = "amount"; `type`: `string` = "uint256" }[] ; `indexed`: `boolean` = false; `internalType`: `string` = "struct ILiqualityHTLC.HTLCData"; `name`: `string` = "htlc"; `type`: `string` = "tuple" })[] ; `name`: `string` = "Initiate"; `outputs`: `undefined` ; `stateMutability`: `undefined` = "view"; `type`: `string` = "event" } \| { `anonymous`: `undefined` = false; `inputs`: { `internalType`: `string` = "bytes32"; `name`: `string` = "id"; `type`: `string` = "bytes32" }[] ; `name`: `string` = "claim"; `outputs`: `any`[] = []; `stateMutability`: `string` = "nonpayable"; `type`: `string` = "function" } \| { `anonymous`: `undefined` = false; `inputs`: { `components`: { `internalType`: `string` = "uint256"; `name`: `string` = "amount"; `type`: `string` = "uint256" }[] ; `internalType`: `string` = "struct ILiqualityHTLC.HTLCData"; `name`: `string` = "htlc"; `type`: `string` = "tuple" }[] ; `name`: `string` = "initiate"; `outputs`: { `internalType`: `string` = "bytes32"; `name`: `string` = ""; `type`: `string` = "bytes32" }[] ; `stateMutability`: `string` = "payable"; `type`: `string` = "function" })[] = `_abi`

#### Defined in

evm/lib/typechain/factories/ILiqualityHTLC__factory.ts:221

## Methods

### connect

▸ `Static` **connect**(`address`, `signerOrProvider`): [`ILiqualityHTLC`](../interfaces/chainify_evm.Typechain.ILiqualityHTLC-1.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `signerOrProvider` | `Provider` \| `Signer` |

#### Returns

[`ILiqualityHTLC`](../interfaces/chainify_evm.Typechain.ILiqualityHTLC-1.md)

#### Defined in

evm/lib/typechain/factories/ILiqualityHTLC__factory.ts:225

___

### createInterface

▸ `Static` **createInterface**(): `ILiqualityHTLCInterface`

#### Returns

`ILiqualityHTLCInterface`

#### Defined in

evm/lib/typechain/factories/ILiqualityHTLC__factory.ts:222
