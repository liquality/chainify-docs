---
id: "chainify_evm.Typechain.IERC721Receiver__factory"
title: "Class: IERC721Receiver__factory"
sidebar_label: "IERC721Receiver__factory"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).IERC721Receiver__factory

## Constructors

### constructor

• **new IERC721Receiver__factory**()

## Properties

### abi

▪ `Static` `Readonly` **abi**: { `inputs`: { `internalType`: `string` = "address"; `name`: `string` = "operator"; `type`: `string` = "address" }[] ; `name`: `string` = "onERC721Received"; `outputs`: { `internalType`: `string` = "bytes4"; `name`: `string` = ""; `type`: `string` = "bytes4" }[] ; `stateMutability`: `string` = "nonpayable"; `type`: `string` = "function" }[] = `_abi`

#### Defined in

evm/lib/typechain/factories/IERC721Receiver__factory.ts:50

## Methods

### connect

▸ `Static` **connect**(`address`, `signerOrProvider`): [`IERC721Receiver`](../interfaces/chainify_evm.Typechain.IERC721Receiver.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `signerOrProvider` | `Provider` \| `Signer` |

#### Returns

[`IERC721Receiver`](../interfaces/chainify_evm.Typechain.IERC721Receiver.md)

#### Defined in

evm/lib/typechain/factories/IERC721Receiver__factory.ts:54

___

### createInterface

▸ `Static` **createInterface**(): `IERC721ReceiverInterface`

#### Returns

`IERC721ReceiverInterface`

#### Defined in

evm/lib/typechain/factories/IERC721Receiver__factory.ts:51
