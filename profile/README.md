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
- [x] Add a throttling feature
- [x] Add a freeze feature for some tokens
- [x] Build a status GH Application
- [x] Redeploy Mailbox on Kadena
- [x] Redeploy all tokens on Kadena
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
- [x] Deploy the WebUI
- [ ] Rotate the admin keys to Multisig on Kadena
- [ ] Rotate the admin keys to Multisig on Ethereum
- [x] Publish all source-code to Etherscan
- [x] Deploy automatic Gas transfer KDA -> ETH

## Current Keys
https://github.com/kinesis-bridge/kadena-hyperlane-keys

## Utility Repositories
Manage and synchronize frontend status with contracts status
https://github.com/kinesis-bridge/hyperlane-kadena-status

Manage Gas relayer account
https://github.com/kinesis-bridge/relayer-gas-manager

## Smart Contracts

#### Common contracts

|                       |    Kadena                                                         |    Ethereum                                              |
|-----------------------|-------------------------------------------------------------------|----------------------------------------------------------|
|  Mailbox              | ``n_e595727b657fbbb3b8e362a05a7bb8d12865c1ff.mailbox``            | ``0x82A729A4c7B2aeBDdbFCCF533e7B75c61c45c23c``           |
|  Validator Announce   | ``n_e595727b657fbbb3b8e362a05a7bb8d12865c1ff.validator-announce`` | ``0xe06ccfFc88f04C3d14355CBD05C85fc238F847Fb``           |
|  Merkle Tree Hook     | ``n_e595727b657fbbb3b8e362a05a7bb8d12865c1ff.merkle-tree-hook``   | ``0xbB7e89E1C475cB02769FfCD8845e5B0B3343ecb7``           |
|  Pausable Hook        |                                                                   | ``0x9e55757C3EF8bcA9015F9d0A6287ccE79215cA07``           |
|  Pausable ISM         |                                                                   | ``0xDeC953FDf8890AEDb5C549dF472A1231baBcE8AC``           |
|  Multisig ISM         | `n_e595727b657fbbb3b8e362a05a7bb8d12865c1ff.merkle-tree-ism``     | ``0x30fE103D354B107635D511134f44fA81D194Fadc`` (Factory) |
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
**Signing Keys for Binaries and Configs:**
```
-----BEGIN PGP PUBLIC KEY BLOCK-----

mQGNBGqj5NUBDADUIsp/aXHnTUUVHrGNxChKS746j/dmTN5iddAMk545jy7BiGOQ
gbL3vgpaAsU/ZUaD7O/vGZAW2eBoYIyGkAXz2w3DCTwWPneBlX9IrqYCxgQwtbRM
Z/vqGx7WjJPNd2VJKaPr1YrVsr4Gx4QRg62QlmTL2Aco0Py91mYreqRZwCPBra1L
s5MNG7xCvfNG6hvSHp9HLmDzS1MYWMIbVFdTiX8jk7HVfHllHQcnON/dIkzNYOqs
pAyAtX35YvWSHBQvLyQ8m4QBi+d0CCjExvbZUqJHSorIlhUIAfTHRECBDCLH1OPY
aY8u0zGEvyN2rZ1U31J/0oW+t3l3XdWO1QdmX3v2mxDnYm4RqlOyTgD1SnvdbFfT
/8ahdJ91C43cHyoxR4PeKgQhFyEHT+kw1Zyu+AstqN2ZqF94Hh0JocPmNsKh4ff9
q5YZfZYLjPSr4pzbrcii7YrP46DGbVqblIGECh9TjsKHMc86oq4PYrpi1e8FNLW/
JFS+M22pekRlcWcAEQEAAbQQS2luc2lzIEJyaWRnZSBDSYkBzgQTAQoAOBYhBGr3
HXofhc2ntIWjsc/RQxedIixxBQJqo+TVAhsDBQsJCAcCBhUKCQgLAgQWAgMBAh4B
AheAAAoJEM/RQxedIixxw5YL/3nlpl0UMcbRHEIXrfdKwBkynqXyylEASWwluSS5
6r96dI0iTuUboKJHCrdo/w/kUSTXcGT17NUYoHJlvCgZLjnIJqHVHtd2CiohvQdN
hHB1KrAxhT5VDf1E4wjUbch2/tPE43b7yF17/hTCUGwemw036k4hP2srNiBx3ge0
3ypic2uFUWpNMNIQlfvJpLAdvsc3DjXMsTAk2GOv0XrBMCzYN9J9gkb7Pmd1gB9H
mgVUS3ysS+FiUjV8VvdifFGgiMUPbiPG0T7J29eGZu5WouiDA+N5EDdBMpXoK4iC
iuladIVwwKnbj7j7esPK8P+h2mvXSFuIAdu9t69QfTf0bfLgyftDhfSBfNOemdfs
eILkUbn9xOSQ+YLvyTeN34CpANII3Jn6iip8Wsfz5x4vBtqxv3GLWwMlQm5nL4VO
fzAuMxvVU0ykvPFysB1ufmH8K482ewfH6GaXtCPIiZQcOO91yHvUCVA4eVaX8xY6
WthEeaXSLH31ZIF7NqULH+57mw==
=ML1W
-----END PGP PUBLIC KEY BLOCK-----
```

```
-----BEGIN PGP PUBLIC KEY BLOCK-----

xjMEaQVgcRYJKwYBBAHaRw8BAQdAnP+ARwxAZm7eGocUhcnqm1qUJ15tlerm
HZGe5j2uzD7NKWtkYV9jb21tdW5pdHlAcG0ubWUgPGtkYV9jb21tdW5pdHlA
cG0ubWU+wsARBBMWCgCDBYJpBWBxAwsJBwkQskGwbEP+TTBFFAAAAAAAHAAg
c2FsdEBub3RhdGlvbnMub3BlbnBncGpzLm9yZynWhsHm/6wEmYBmGXzpU1I9
X9iQKz4kUsw72A4GJ/pdAxUKCAQWAAIBAhkBApsDAh4BFiEEZQoREsXC0He0
eUpuskGwbEP+TTAAALyJAQDsFbzDLA5xn4UuJVVDgX/cBF97x3hFz1ZAGIiX
cRyf4gEAs8Ck3eubr60pNbP7LX9eEEL2tCReNu0pbDWr9kTZnAnOOARpBWBx
EgorBgEEAZdVAQUBAQdAKkGBUmJJ+Ji2jaMf2Nu87vEjsl7W7ufHfH6XsVPr
ogsDAQgHwr4EGBYKAHAFgmkFYHEJELJBsGxD/k0wRRQAAAAAABwAIHNhbHRA
bm90YXRpb25zLm9wZW5wZ3Bqcy5vcmeT7PAYAfk7R+9v5uVskDsM3NsdjxLZ
a0M0avy8nmt1BAKbDBYhBGUKERLFwtB3tHlKbrJBsGxD/k0wAABuxwD+JIy7
iexBt/OjX85rylB9pC/Jr0dKVrb53BH8aorYxCIBAO+F5R/7SXC9at+xhYmQ
n1GlLUN818skrBci1iN/z9II
=YPDb
-----END PGP PUBLIC KEY BLOCK-----
```

