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
- [x] Do some changes on the Kadena Multi-Sig ISM (set-threshood function)
- [x] Deploy the new Kadena Multi-Sig ISM
- [x] Fix Gas usage on DomainRouting ISM
- [x] Redeploy DomainRouting
- [x] Add a chain translator feature
- [ ] Add a throttling feature
- [ ] Add a freeze feature for some tokens
- [x] Build a status GH Application
- [x] Redeploy Mailbox on Kadena
- [ ] Redeploy all tokens on Kadena
- [x] Prepare a S3 storage
- [x] Deploy a pair of temporary validators
- [x] Deploy the relayer
- [x] Rotate the ISM Multisig On Ethereum => To a temporary validator
- [x] Rotate the ISM Multisig on Kadena => To a temporary validation
- [x] Prepare and deploy a Validator 
- [ ] Deploy production grade validators WIP
- [ ] Rotate the ISM Multisig On Ethereum => To final validators set  WIP
- [ ] Rotate the ISM Multisig on Kadena => To final validators set WIP
- [x] Disable the Backend on the WebUI
- [ ] Deploy the WebUI
- [ ] Rotate the admin keys to Multisig on Kadena
- [ ] Rotate the admin keys to Multisig on Ethereum
- [x] Publish all source-code to Etherscan

## Current Keys
https://github.com/kinesis-bridge/kadena-hyperlane-keys


## Smart Contracts

#### Common contracts

|                       |    Kadena                                                         |    Ethereum                                              |
|-----------------------|-------------------------------------------------------------------|----------------------------------------------------------|
|  Mailbox              | ``n_e595727b657fbbb3b8e362a05a7bb8d12865c1ff.mailbox``            | ``0x82A729A4c7B2aeBDdbFCCF533e7B75c61c45c23c``           |
|  Validator Announce   | ``n_e595727b657fbbb3b8e362a05a7bb8d12865c1ff.validator-announce`` | ``0xe06ccfFc88f04C3d14355CBD05C85fc238F847Fb``           |
|  Merkle Tree Hook     | ``n_e595727b657fbbb3b8e362a05a7bb8d12865c1ff.merkle-tree-hook``   | ``0xbB7e89E1C475cB02769FfCD8845e5B0B3343ecb7``           |
|  Pausable Hook        |                                                                   | ``0x9e55757C3EF8bcA9015F9d0A6287ccE79215cA07``           |
|  Multisig ISM         | ``n_e595727b657fbbb3b8e362a05a7bb8d12865c1ff.merkle-tree-ism``    | ``0x35Acc909526f6670c02d52552147Dc05b0dc2aC0`` (Proxy)   |
|    -                  |                                                                   | ``0x3904BCf13fcBa7C8d0849cf344d453Fc0F53cb02`` (Impl)    |
| Pausable ISM          |                                                                   | ``0xDeC953FDf8890AEDb5C549dF472A1231baBcE8AC``           |
| Multisig ISM          |                                                                   | ``0x30fE103D354B107635D511134f44fA81D194Fadc`` (Factory) |
|    -                  |                                                                   | ``0x3904BCf13fcBa7C8d0849cf344d453Fc0F53cb02`` (Impl)    |
|    -                  |                                                                   | ``0xcE0963E5759B37750e6b0aF5DFce6384B73E1d01`` (Proxy)   |
| Aggregation ISM       |                                                                   | ``0xb3D7E5B97d4f47B7eD8503d5c2e5CcC7CCB07591`` (Factory) |
|    -                  |                                                                   | ``0x2D56168d3110F378b9BC598683423210c1A957BC`` (Impl)    |
|    -                  |                                                                   | ``0x82EE09AC5616FD7d53bEC4dAf99f1c4f1B104dF4`` (Proxy)   |

---


#### Native Kadena Tokens (Collateral on Kadena side)

|                       |    Kadena                                                         |    Ethereum                                              |
|-----------------------|-------------------------------------------------------------------|----------------------------------------------------------|
| KDA                   | ``n_e595727b657fbbb3b8e362a05a7bb8d12865c1ff.KDA``                | ``0x7786F1eb2eC198A04d8f5e3Fc36fAB14da370076`` (Proxy)   |
|   -                   | ``c:TLKMz0rO15FnZARzjvdoT6FHMGWqc8NGI0V_p2KvjY4`` (Coll Account)  | ``0x0009C43128dC38bF92cfA5e628f69215fe98a705`` (Impl)    |

---

#### Ethereum Collateralized Tokens (Collateral on Ethereum side)

|                       |    Kadena                                                         |    Ethereum                                              |
|-----------------------|-------------------------------------------------------------------|----------------------------------------------------------|
| USDC                  | ``n_e595727b657fbbb3b8e362a05a7bb8d12865c1ff.kb-USDC``            | ``0x81C2813aa88F66bca1e55838045Aaceb72FEbFc1`` (Proxy)   |
|   -                   |                                                                   | ``0xb0d6EED90f8E497b867F557C44A49c8c81Fa0a5D`` (Impl)    |
| ETH                   | ``n_e595727b657fbbb3b8e362a05a7bb8d12865c1ff.kb-ETH``             | ``0xbddB58bF21b12D70eED91b939Ae061572010B11d`` (Proxy)   |
|   -                   |                                                                   | ``0x941232cAD238BC5b897561BFF8E2b16bfA3945BA`` (Impl)    |
| WBTC                  | ``n_e595727b657fbbb3b8e362a05a7bb8d12865c1ff.kb-WBTC``            | ``0xDFdB8F3dEb5458BFA25cc97df41298A915a34BF3`` (Proxy)   |
|   -                   |                                                                   | ``0xC5fA6A9cCccc14adb0576a37d96A9BEcF68cA0e3`` (Impl)    |


---
