---
id: "chainify_evm.Typechain.IERC1155Receiver__factory"
title: "Class: IERC1155Receiver__factory"
sidebar_label: "IERC1155Receiver__factory"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).IERC1155Receiver__factory

## Constructors

### constructor

• **new IERC1155Receiver__factory**()

## Properties

### abi

▪ `Static` `Readonly` **abi**: { `inputs`: { `internalType`: `string` = "address"; `name`: `string` = "operator"; `type`: `string` = "address" }[] ; `name`: `string` = "onERC1155BatchReceived"; `outputs`: { `internalType`: `string` = "bytes4"; `name`: `string` = ""; `type`: `string` = "bytes4" }[] ; `stateMutability`: `string` = "nonpayable"; `type`: `string` = "function" }[] = `_abi`

#### Defined in

evm/lib/typechain/factories/IERC1155Receiver__factory.ts:113

## Methods

### connect

▸ `Static` **connect**(`address`, `signerOrProvider`): [`IERC1155Receiver`](../interfaces/chainify_evm.Typechain.IERC1155Receiver.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `signerOrProvider` | `Provider` \| `Signer` |

#### Returns

[`IERC1155Receiver`](../interfaces/chainify_evm.Typechain.IERC1155Receiver.md)

#### Defined in

evm/lib/typechain/factories/IERC1155Receiver__factory.ts:117

___

### createInterface

▸ `Static` **createInterface**(): `IERC1155ReceiverInterface`

#### Returns

`IERC1155ReceiverInterface`

#### Defined in

evm/lib/typechain/factories/IERC1155Receiver__factory.ts:114
