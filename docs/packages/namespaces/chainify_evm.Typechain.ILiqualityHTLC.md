---
id: "chainify_evm.Typechain.ILiqualityHTLC"
title: "Namespace: ILiqualityHTLC"
sidebar_label: "ILiqualityHTLC"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](chainify_evm.Typechain.md).ILiqualityHTLC

## Type aliases

### HTLCDataStruct

Ƭ **HTLCDataStruct**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `amount` | `BigNumberish` |
| `expiration` | `BigNumberish` |
| `recipientAddress` | `string` |
| `refundAddress` | `string` |
| `secretHash` | `BytesLike` |
| `tokenAddress` | `string` |

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:22

___

### HTLCDataStructOutput

Ƭ **HTLCDataStructOutput**: [`BigNumber`, `BigNumber`, `string`, `string`, `string`, `string`] & { `amount`: `BigNumber` ; `expiration`: `BigNumber` ; `recipientAddress`: `string` ; `refundAddress`: `string` ; `secretHash`: `string` ; `tokenAddress`: `string`  }

#### Defined in

evm/lib/typechain/ILiqualityHTLC.ts:31
