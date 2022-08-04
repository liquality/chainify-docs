---
id: "chainify_terra.TerraTypes.TerraTxRequest"
title: "Interface: TerraTxRequest"
sidebar_label: "TerraTxRequest"
custom_edit_url: null
---

[@chainify/terra](../modules/chainify_terra.md).[TerraTypes](../namespaces/chainify_terra.TerraTypes.md).TerraTxRequest

## Hierarchy

- `TransactionRequest`

  ↳ **`TerraTxRequest`**

## Properties

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

#### Overrides

TransactionRequest.gasLimit

#### Defined in

[terra/lib/types/index.ts:17](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/types/index.ts#L17)

___

### memo

• `Optional` **memo**: `string`

#### Defined in

[terra/lib/types/index.ts:16](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/types/index.ts#L16)

___

### msgs

• `Optional` **msgs**: `Msg`[]

#### Defined in

[terra/lib/types/index.ts:15](https://github.com/liquality/chainify/blob/540cfa69/packages/terra/lib/types/index.ts#L15)

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
