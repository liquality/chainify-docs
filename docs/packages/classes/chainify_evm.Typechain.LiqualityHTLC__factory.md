---
id: "chainify_evm.Typechain.LiqualityHTLC__factory"
title: "Class: LiqualityHTLC__factory"
sidebar_label: "LiqualityHTLC__factory"
custom_edit_url: null
---

[@chainify/evm](../modules/chainify_evm.md).[Typechain](../namespaces/chainify_evm.Typechain.md).LiqualityHTLC__factory

## Hierarchy

- `ContractFactory`

  ↳ **`LiqualityHTLC__factory`**

## Constructors

### constructor

• **new LiqualityHTLC__factory**(...`args`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `...args` | `LiqualityHTLCConstructorParams` |

#### Overrides

ContractFactory.constructor

#### Defined in

evm/lib/typechain/factories/LiqualityHTLC__factory.ts:272

## Properties

### contractName

• `Readonly` **contractName**: ``"LiqualityHTLC"``

#### Defined in

evm/lib/typechain/factories/LiqualityHTLC__factory.ts:298

___

### abi

▪ `Static` `Readonly` **abi**: ({ `anonymous`: `undefined` = false; `inputs`: `any`[] = []; `name`: `string` = "LiqualityHTLC\_\_InvalidExpiration"; `outputs`: `undefined` ; `stateMutability`: `undefined` = "view"; `type`: `string` = "error" } \| { `anonymous`: `boolean` = false; `inputs`: ({ `components`: `undefined` ; `indexed`: `boolean` = false; `internalType`: `string` = "bytes32"; `name`: `string` = "id"; `type`: `string` = "bytes32" } \| { `components`: { `internalType`: `string` = "uint256"; `name`: `string` = "amount"; `type`: `string` = "uint256" }[] ; `indexed`: `boolean` = false; `internalType`: `string` = "struct ILiqualityHTLC.HTLCData"; `name`: `string` = "htlc"; `type`: `string` = "tuple" })[] ; `name`: `string` = "Initiate"; `outputs`: `undefined` ; `stateMutability`: `undefined` = "view"; `type`: `string` = "event" } \| { `anonymous`: `undefined` = false; `inputs`: { `internalType`: `string` = "bytes32"; `name`: `string` = ""; `type`: `string` = "bytes32" }[] ; `name`: `string` = "htlcs"; `outputs`: { `internalType`: `string` = "uint256"; `name`: `string` = "amount"; `type`: `string` = "uint256" }[] ; `stateMutability`: `string` = "view"; `type`: `string` = "function" } \| { `anonymous`: `undefined` = false; `inputs`: { `components`: { `internalType`: `string` = "uint256"; `name`: `string` = "amount"; `type`: `string` = "uint256" }[] ; `internalType`: `string` = "struct ILiqualityHTLC.HTLCData"; `name`: `string` = "htlc"; `type`: `string` = "tuple" }[] ; `name`: `string` = "initiate"; `outputs`: { `internalType`: `string` = "bytes32"; `name`: `string` = "id"; `type`: `string` = "bytes32" }[] ; `stateMutability`: `string` = "payable"; `type`: `string` = "function" })[] = `_abi`

#### Defined in

evm/lib/typechain/factories/LiqualityHTLC__factory.ts:300

___

### bytecode

▪ `Static` `Readonly` **bytecode**: ``"0x608060405234801561001057600080fd5b50610cfd806100206000396000f3fe60806040526004361061003f5760003560e01c8063337bc2fa146100445780637249fbb61461006a57806384cc9dfb1461008c57806391edd8f2146100ac575b600080fd5b610057610052366004610a95565b610147565b6040519081526020015b60405180910390f35b34801561007657600080fd5b5061008a610085366004610aad565b61036d565b005b34801561009857600080fd5b5061008a6100a7366004610ac6565b6104c8565b3480156100b857600080fd5b5061010b6100c7366004610aad565b6000602081905290815260409020805460018201546002830154600384015460048501546005909501549394929391926001600160a01b0391821692908216911686565b604080519687526020870195909552938501929092526001600160a01b03908116606085015290811660808401521660a082015260c001610061565b6000428260200135101561016e5760405163e7ec8bc960e01b815260040160405180910390fd5b813561018d57604051639f7fe22f60e01b815260040160405180910390fd5b600061019f6080840160608501610b00565b6001600160a01b031614156101d457813534146101cf576040516309a9fccd60e01b815260040160405180910390fd5b61021b565b34156101f3576040516309a9fccd60e01b815260040160405180910390fd5b61021b3330843561020a6080870160608801610b00565b6001600160a01b03169291906106a0565b600261022d60a0840160808501610b00565b4284356020860135604087013561024a60c0890160a08a01610b00565b604080516001600160a01b039788166020820152908101959095526060850193909352608084019190915260a083015290911660c082015260e00160408051601f198184030181529082905261029f91610b49565b602060405180830381855afa1580156102bc573d6000803e3d6000fd5b5050506040513d601f19601f820116820180604052508101906102df9190610b65565b600081815260208190526040902060010154909150156103125760405163908b86b760e01b815260040160405180910390fd5b6000818152602081905260409020829061032c8282610b7e565b9050507f3c07675a13dc2c3d44c781f9dd3db9ac3a9cc543a5f46777f7bd60a942cf6eb78183604051610360929190610c1e565b60405180910390a1919050565b60008181526020818152604091829020825160c08101845281548152600182015492810183905260028201549381019390935260038101546001600160a01b0390811660608501526004820154811660808501526005909101541660a08301526103ea5760405163501a3cef60e11b815260040160405180910390fd5b8060200151421161040e576040516377128aa160e11b815260040160405180910390fd5b60008281526020819052604080822082815560018101839055600281018390556003810180546001600160a01b0319908116909155600482018054821690556005909101805490911690555183917f3fbd469ec3a5ce074f975f76ce27e727ba21c99176917b97ae2e713695582a1291a260608101516001600160a01b03166104a7576104a38160800151826000015161073e565b5050565b6080810151815160608301516104a3926001600160a01b03909116916107e6565b60008281526020818152604091829020825160c08101845281548152600182015492810183905260028201549381019390935260038101546001600160a01b0390811660608501526004820154811660808501526005909101541660a08301526105455760405163501a3cef60e11b815260040160405180910390fd5b806040015160028360405160200161055f91815260200190565b60408051601f198184030181529082905261057991610b49565b602060405180830381855afa158015610596573d6000803e3d6000fd5b5050506040513d601f19601f820116820180604052508101906105b99190610b65565b146105d7576040516392631d5760e01b815260040160405180910390fd5b6000838152602081815260408083208381556001810184905560028101939093556003830180546001600160a01b03199081169091556004840180548216905560059093018054909316909255905183815284917f5664142af3dcfc3dc3de45a43f75c746bd1d8c11170a5037fdf98bdb35775137910160405180910390a260608101516001600160a01b031661067f5761067a8160a00151826000015161073e565b505050565b60a08101518151606083015161067a926001600160a01b03909116916107e6565b6040516001600160a01b03808516602483015283166044820152606481018290526107389085906323b872dd60e01b906084015b60408051601f198184030181529190526020810180517bffffffffffffffffffffffffffffffffffffffffffffffffffffffff167fffffffff0000000000000000000000000000000000000000000000000000000090931692909217909152610816565b50505050565b6000826001600160a01b03168260405160006040518083038185875af1925050503d806000811461078b576040519150601f19603f3d011682016040523d82523d6000602084013e610790565b606091505b505090508061067a5760405162461bcd60e51b815260206004820152600f60248201527f7472616e73666572206661696c6564000000000000000000000000000000000060448201526064015b60405180910390fd5b6040516001600160a01b03831660248201526044810182905261067a90849063a9059cbb60e01b906064016106d4565b600061086b826040518060400160405280602081526020017f5361666545524332303a206c6f772d6c6576656c2063616c6c206661696c6564815250856001600160a01b03166108fb9092919063ffffffff16565b80519091501561067a57808060200190518101906108899190610c9b565b61067a5760405162461bcd60e51b815260206004820152602a60248201527f5361666545524332303a204552433230206f7065726174696f6e20646964206e60448201527f6f7420737563636565640000000000000000000000000000000000000000000060648201526084016107dd565b606061090a8484600085610914565b90505b9392505050565b60608247101561098c5760405162461bcd60e51b815260206004820152602660248201527f416464726573733a20696e73756666696369656e742062616c616e636520666f60448201527f722063616c6c000000000000000000000000000000000000000000000000000060648201526084016107dd565b6001600160a01b0385163b6109e35760405162461bcd60e51b815260206004820152601d60248201527f416464726573733a2063616c6c20746f206e6f6e2d636f6e747261637400000060448201526064016107dd565b600080866001600160a01b031685876040516109ff9190610b49565b60006040518083038185875af1925050503d8060008114610a3c576040519150601f19603f3d011682016040523d82523d6000602084013e610a41565b606091505b5091509150610a51828286610a5c565b979650505050505050565b60608315610a6b57508161090d565b825115610a7b5782518084602001fd5b8160405162461bcd60e51b81526004016107dd9190610cbd565b600060c08284031215610aa757600080fd5b50919050565b600060208284031215610abf57600080fd5b5035919050565b60008060408385031215610ad957600080fd5b50508035926020909101359150565b6001600160a01b0381168114610afd57600080fd5b50565b600060208284031215610b1257600080fd5b813561090d81610ae8565b60005b83811015610b38578181015183820152602001610b20565b838111156107385750506000910152565b60008251610b5b818460208701610b1d565b9190910192915050565b600060208284031215610b7757600080fd5b5051919050565b8135815560208201356001820155604082013560028201556060820135610ba481610ae8565b6003820180546001600160a01b0319166001600160a01b038316179055506080820135610bd081610ae8565b6004820180546001600160a01b0319166001600160a01b0383161790555060a0820135610bfc81610ae8565b6005820180546001600160a01b0319166001600160a01b038316179055505050565b600060e0820190508382528235602083015260208301356040830152604083013560608301526060830135610c5281610ae8565b6001600160a01b03808216608085015260808501359150610c7282610ae8565b80821660a085015260a08501359150610c8a82610ae8565b80821660c085015250509392505050565b600060208284031215610cad57600080fd5b8151801515811461090d57600080fd5b6020815260008251806020840152610cdc816040850160208701610b1d565b601f01601f1916919091016040019291505056fea164736f6c634300080b000a"``

#### Defined in

evm/lib/typechain/factories/LiqualityHTLC__factory.ts:299

___

### contractName

▪ `Static` `Readonly` **contractName**: ``"LiqualityHTLC"``

#### Defined in

evm/lib/typechain/factories/LiqualityHTLC__factory.ts:297

## Methods

### attach

▸ **attach**(`address`): [`LiqualityHTLC`](../interfaces/chainify_evm.Typechain.LiqualityHTLC.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |

#### Returns

[`LiqualityHTLC`](../interfaces/chainify_evm.Typechain.LiqualityHTLC.md)

#### Overrides

ContractFactory.attach

#### Defined in

evm/lib/typechain/factories/LiqualityHTLC__factory.ts:291

___

### connect

▸ **connect**(`signer`): [`LiqualityHTLC__factory`](chainify_evm.Typechain.LiqualityHTLC__factory.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `signer` | `Signer` |

#### Returns

[`LiqualityHTLC__factory`](chainify_evm.Typechain.LiqualityHTLC__factory.md)

#### Overrides

ContractFactory.connect

#### Defined in

evm/lib/typechain/factories/LiqualityHTLC__factory.ts:294

___

### deploy

▸ **deploy**(`overrides?`): `Promise`<[`LiqualityHTLC`](../interfaces/chainify_evm.Typechain.LiqualityHTLC.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `overrides?` | `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`Promise`<[`LiqualityHTLC`](../interfaces/chainify_evm.Typechain.LiqualityHTLC.md)\>

#### Overrides

ContractFactory.deploy

#### Defined in

evm/lib/typechain/factories/LiqualityHTLC__factory.ts:281

___

### getDeployTransaction

▸ **getDeployTransaction**(`overrides?`): `TransactionRequest`

#### Parameters

| Name | Type |
| :------ | :------ |
| `overrides?` | `Overrides` & { `from?`: `string` \| `Promise`<`string`\>  } |

#### Returns

`TransactionRequest`

#### Overrides

ContractFactory.getDeployTransaction

#### Defined in

evm/lib/typechain/factories/LiqualityHTLC__factory.ts:286

___

### connect

▸ `Static` **connect**(`address`, `signerOrProvider`): [`LiqualityHTLC`](../interfaces/chainify_evm.Typechain.LiqualityHTLC.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |
| `signerOrProvider` | `Provider` \| `Signer` |

#### Returns

[`LiqualityHTLC`](../interfaces/chainify_evm.Typechain.LiqualityHTLC.md)

#### Defined in

evm/lib/typechain/factories/LiqualityHTLC__factory.ts:304

___

### createInterface

▸ `Static` **createInterface**(): `LiqualityHTLCInterface`

#### Returns

`LiqualityHTLCInterface`

#### Defined in

evm/lib/typechain/factories/LiqualityHTLC__factory.ts:301