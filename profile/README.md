# Kinesis Bridge Community : kadena <-> Ethereum

## Tasks

- [x] Recover keys from 4Pto
- [x] Recover and publish source code
- [x] Rotate the admin / pausing keys
- [x] Deploy and activate new ISM Pause Contract
- [x] Divide authorization between Admin, Relayer, Validators on Kadena,  create associated accounts.
- [x] Deploy and plug a Hook Pause contract
- [x] Disable IGP Hook on Ethereum
- [x] Rewrite the Kadena IGP with KIA
- [x] Deploy the new IGP on Kadena
- [x] Do some changes on the Kadena Multi-Sig ISM (set-threshoold function)
- [x] Deploy yhe new Kadena Multi-Sig ISM
- [x] Fix Gas usage on DomainRouting ISM
- [x] Redeploy DomainRouting
- [x] Add a chain translator feature
- [ ] Add a throtlling feature
- [ ] Add a freeze feature for some tokens
- [ ] Build a status GH Application
- [x] Redeploy Mailbox on Kadena
- [ ] Redeploy all tokens on Kadena
- [x] Prepare a S3 storage
- [x] Deploy a pair of temporary validators
- [x] Deploy the relayer
- [x] Rotate the ISM MultiSig On Ethereum => To a temporay validator
- [x] Rotate the ISM MultiSig on Kadena => To a temporary validation
- [x] Prepare and deploy a Validator 
- [ ] Deploy production grade validators WIP
- [ ] Rotate the ISM MultiSig On Ethereum => To final validators set  WIP
- [ ] Rotate the ISM MultiSig on Kadena => To final validators set WIP
- [ ] Disable the Backend on the WebUI
- [ ] Deploy the WebUI
- [ ] Rotate the admin keys to MultSig on Kadena
- [ ] Rotate the admin keys to MultiSig on Ethereum
- [x] Publish all source-code to Etherscan

## Current Keys
https://github.com/kinesis-bridge/kadena-hyperlane-keys


## Smart Contracts

Common contracts.
TBC

|                       |    Kadena                                                     |    Ethereum                                            |
|-----------------------|---------------------------------------------------------------|--------------------------------------------------------|
|  Mailbox              | n_e595727b657fbbb3b8e362a05a7bb8d12865c1ff.mailbox            | 0x82A729A4c7B2aeBDdbFCCF533e7B75c61c45c23c             |
|  Validator Announce   | n_e595727b657fbbb3b8e362a05a7bb8d12865c1ff.validator-announce | 0xe06ccfFc88f04C3d14355CBD05C85fc238F847Fb             |
|  Merkle Tree Hook     | n_e595727b657fbbb3b8e362a05a7bb8d12865c1ff.merkle-tree-hook   | 0xbB7e89E1C475cB02769FfCD8845e5B0B3343ecb7             |
|  Multisig ISM         | n_e595727b657fbbb3b8e362a05a7bb8d12865c1ff.merkle-tree-ism    | 0x35Acc909526f6670c02d52552147Dc05b0dc2aC0 (Proxy)     |
|    -                  |                                                               | 0x3904BCf13fcBa7C8d0849cf344d453Fc0F53cb02 (Impl)      |
| Pausable ISM          |                                                               |  0xDeC953FDf8890AEDb5C549dF472A1231baBcE8AC            |
| MultiSig ISM          |                                                               | 0x30fE103D354B107635D511134f44fA81D194Fadc (Factory)   |
|    -                  |                                                               | 0x3904BCf13fcBa7C8d0849cf344d453Fc0F53cb02 (Impl)      |
|    -                  |                                                               | 0xcE0963E5759B37750e6b0aF5DFce6384B73E1d01 (Proxy)     |
| Aggregation ISM       |                                                               | 0xb3D7E5B97d4f47B7eD8503d5c2e5CcC7CCB07591 (Factory)   |
|    -                  |                                                               | 0x2D56168d3110F378b9BC598683423210c1A957BC (Impl)      |
|    -                  |                                                               | 0x82EE09AC5616FD7d53bEC4dAf99f1c4f1B104dF4 (Proxy)     |
