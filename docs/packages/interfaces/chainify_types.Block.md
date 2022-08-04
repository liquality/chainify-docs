---
id: "chainify_types.Block"
title: "Interface: Block<BlockType, TransactionType>"
sidebar_label: "Block"
custom_edit_url: null
---

[@chainify/types](../modules/chainify_types.md).Block

## Type parameters

| Name | Type |
| :------ | :------ |
| `BlockType` | `any` |
| `TransactionType` | `any` |

## Properties

### \_raw

• **\_raw**: `BlockType`

#### Defined in

[types/lib/Block.ts:21](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Block.ts#L21)

___

### difficulty

• `Optional` **difficulty**: `number`

#### Defined in

[types/lib/Block.ts:13](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Block.ts#L13)

___

### hash

• **hash**: `string`

#### Defined in

[types/lib/Block.ts:7](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Block.ts#L7)

___

### nonce

• `Optional` **nonce**: `number`

#### Defined in

[types/lib/Block.ts:15](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Block.ts#L15)

___

### number

• **number**: `number`

#### Defined in

[types/lib/Block.ts:5](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Block.ts#L5)

___

### parentHash

• `Optional` **parentHash**: `string`

#### Defined in

[types/lib/Block.ts:11](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Block.ts#L11)

___

### size

• `Optional` **size**: `number`

#### Defined in

[types/lib/Block.ts:17](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Block.ts#L17)

___

### timestamp

• **timestamp**: `number`

#### Defined in

[types/lib/Block.ts:9](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Block.ts#L9)

___

### transactions

• `Optional` **transactions**: [`Transaction`](chainify_types.Transaction.md)<`TransactionType`\>[]

#### Defined in

[types/lib/Block.ts:19](https://github.com/liquality/chainify/blob/540cfa69/packages/types/lib/Block.ts#L19)
