---
id: "chainify_near.NearTypes.NearTxRequest"
title: "Interface: NearTxRequest"
sidebar_label: "NearTxRequest"
custom_edit_url: null
---

[@chainify/near](../modules/chainify_near.md).[NearTypes](../namespaces/chainify_near.NearTypes.md).NearTxRequest

## Hierarchy

- `TransactionRequest`

  ↳ **`NearTxRequest`**

## Properties

### actions

• `Optional` **actions**: `Action`[]

#### Defined in

[near/lib/types.ts:49](https://github.com/liquality/chainify/blob/540cfa69/packages/near/lib/types.ts#L49)

___

### asset

• `Optional` **asset**: `Asset`

#### Inherited from

TransactionRequest.asset

#### Defined in

types/dist/lib/Transaction.d.ts:29

___

### data

• `Optional` **data**: `string`

#### Inherited from

TransactionRequest.data

#### Defined in

types/dist/lib/Transaction.d.ts:32

___

### fee

• `Optional` **fee**: `FeeType`

#### Inherited from

TransactionRequest.fee

#### Defined in

types/dist/lib/Transaction.d.ts:34

___

### feeAsset

• `Optional` **feeAsset**: `Asset`

#### Inherited from

TransactionRequest.feeAsset

#### Defined in

types/dist/lib/Transaction.d.ts:30

___

### gasLimit

• `Optional` **gasLimit**: `number`

#### Inherited from

TransactionRequest.gasLimit

#### Defined in

types/dist/lib/Transaction.d.ts:35

___

### to

• `Optional` **to**: `AddressType`

#### Inherited from

TransactionRequest.to

#### Defined in

types/dist/lib/Transaction.d.ts:31

___

### value

• `Optional` **value**: `BigNumber`

#### Inherited from

TransactionRequest.value

#### Defined in

types/dist/lib/Transaction.d.ts:33
