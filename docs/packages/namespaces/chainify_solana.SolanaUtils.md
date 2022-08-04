---
id: "chainify_solana.SolanaUtils"
title: "Namespace: SolanaUtils"
sidebar_label: "SolanaUtils"
custom_edit_url: null
---

[@chainify/solana](../modules/chainify_solana.md).SolanaUtils

## Functions

### parseBlockResponse

▸ **parseBlockResponse**(`data`): `Block`

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | `BlockResponse` |

#### Returns

`Block`

#### Defined in

[solana/lib/utils.ts:5](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/utils.ts#L5)

___

### parseTransactionResponse

▸ **parseTransactionResponse**(`data`, `signatures?`): `Transaction`

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | `ParsedTransactionWithMeta` |
| `signatures?` | `RpcResponseAndContext`<`SignatureStatus`\> |

#### Returns

`Transaction`

#### Defined in

[solana/lib/utils.ts:15](https://github.com/liquality/chainify/blob/540cfa69/packages/solana/lib/utils.ts#L15)
