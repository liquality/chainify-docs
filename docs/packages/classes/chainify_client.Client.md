---
id: "chainify_client.Client"
title: "Class: Client<ChainType, WalletType, SwapType, NftType>"
sidebar_label: "Client"
custom_edit_url: null
---

[@chainify/client](../modules/chainify_client.md).Client

## Type parameters

| Name | Type |
| :------ | :------ |
| `ChainType` | extends [`Chain`](chainify_client.Chain.md)<`any`\> = [`Chain`](chainify_client.Chain.md)<`any`\> |
| `WalletType` | extends [`Wallet`](chainify_client.Wallet.md)<`any`, `any`\> = [`Wallet`](chainify_client.Wallet.md)<`any`, `any`\> |
| `SwapType` | extends [`Swap`](chainify_client.Swap.md)<`any`, `any`\> = [`Swap`](chainify_client.Swap.md)<`any`, `any`\> |
| `NftType` | extends [`Nft`](chainify_client.Nft.md)<`any`, `any`\> = [`Nft`](chainify_client.Nft.md)<`any`, `any`\> |

## Constructors

### constructor

• **new Client**<`ChainType`, `WalletType`, `SwapType`, `NftType`\>(`chain?`, `wallet?`, `swap?`, `nft?`)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `ChainType` | extends [`Chain`](chainify_client.Chain.md)<`any`, `Network`, `ChainType`\> = [`Chain`](chainify_client.Chain.md)<`any`, `Network`\> |
| `WalletType` | extends [`Wallet`](chainify_client.Wallet.md)<`any`, `any`, `WalletType`\> = [`Wallet`](chainify_client.Wallet.md)<`any`, `any`\> |
| `SwapType` | extends [`Swap`](chainify_client.Swap.md)<`any`, `any`, [`Wallet`](chainify_client.Wallet.md)<`any`, `any`\>, `SwapType`\> = [`Swap`](chainify_client.Swap.md)<`any`, `any`, [`Wallet`](chainify_client.Wallet.md)<`any`, `any`\>\> |
| `NftType` | extends [`Nft`](chainify_client.Nft.md)<`any`, `any`, `NftType`\> = [`Nft`](chainify_client.Nft.md)<`any`, `any`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `chain?` | `ChainType` |
| `wallet?` | `WalletType` |
| `swap?` | `SwapType` |
| `nft?` | `NftType` |

#### Defined in

[client/lib/Client.ts:17](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Client.ts#L17)

## Accessors

### chain

• `get` **chain**(): `ChainType`

#### Returns

`ChainType`

#### Defined in

[client/lib/Client.ts:72](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Client.ts#L72)

• `set` **chain**(`chain`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `chain` | `ChainType` |

#### Returns

`void`

#### Defined in

[client/lib/Client.ts:76](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Client.ts#L76)

___

### nft

• `get` **nft**(): `NftType`

#### Returns

`NftType`

#### Defined in

[client/lib/Client.ts:96](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Client.ts#L96)

• `set` **nft**(`nft`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `nft` | `NftType` |

#### Returns

`void`

#### Defined in

[client/lib/Client.ts:100](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Client.ts#L100)

___

### swap

• `get` **swap**(): `SwapType`

#### Returns

`SwapType`

#### Defined in

[client/lib/Client.ts:88](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Client.ts#L88)

• `set` **swap**(`swap`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `swap` | `SwapType` |

#### Returns

`void`

#### Defined in

[client/lib/Client.ts:92](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Client.ts#L92)

___

### wallet

• `get` **wallet**(): `WalletType`

#### Returns

`WalletType`

#### Defined in

[client/lib/Client.ts:80](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Client.ts#L80)

• `set` **wallet**(`wallet`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `wallet` | `WalletType` |

#### Returns

`void`

#### Defined in

[client/lib/Client.ts:84](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Client.ts#L84)

## Methods

### connect

▸ **connect**(`provider`): [`Client`](chainify_client.Client.md)<`ChainType`, `WalletType`, `SwapType`, `NftType`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `provider` | `ChainType` \| `WalletType` \| `SwapType` \| `NftType` |

#### Returns

[`Client`](chainify_client.Client.md)<`ChainType`, `WalletType`, `SwapType`, `NftType`\>

#### Defined in

[client/lib/Client.ts:24](https://github.com/liquality/chainify/blob/540cfa69/packages/client/lib/Client.ts#L24)
