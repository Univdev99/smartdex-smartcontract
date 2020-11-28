This repository is forked from [0x-monorepo](https://github.com/0xProject/0x-monorepo)                 |

## Usage

Node version 6.x or 8.x is required.

Most of the packages require additional typings for external dependencies.
You can include those by prepending the `@0x/typescript-typings` package to your [`typeRoots`](http://www.typescriptlang.org/docs/handbook/tsconfig-json.html) config.

```json
"typeRoots": ["node_modules/@0x/typescript-typings/types", "node_modules/@types"],
```

## Contributing

We strongly recommend that the community help us make improvements and determine the future direction of the protocol. To report bugs within this package, please create an issue in this repository.

#### Read our [contribution guidelines](./CONTRIBUTING.md).

### Install dependencies

Make sure you are using Yarn v1.9.4. To install using brew:

```bash
brew install yarn@1.9.4
```

Then install dependencies

```bash
yarn install
```

You will also need to have Python 3 installed, in order to build and run the tests of `abi-gen`'s command-line interface, which is integrated with the yarn build, yarn test, and yarn lint commands described below. More specifically, your local pip should resolve to the Python 3 version of pip, not a Python 2.x version.

### Build

To build all packages:

```bash
yarn build
```

To build a specific package:

```bash
PKG=@0x/web3-wrapper yarn build
```

To build all contracts packages:

```bash
yarn build:contracts
```

### Watch

To re-build all packages on change:

```bash
yarn watch
```

To watch a specific package and all it's dependent packages:

```bash
PKG=[NPM_PACKAGE_NAME] yarn watch

e.g
PKG=@0x/web3-wrapper yarn watch
```

### Clean

Clean all packages:

```bash
yarn clean
```

Clean a specific package

```bash
PKG=0x.js yarn clean
```

### Rebuild

To re-build (clean & build) all packages:

```bash
yarn rebuild
```

To re-build (clean & build) a specific package & it's deps:

```bash
PKG=0x.js yarn rebuild
```

### Lint

Lint all packages:

```bash
yarn lint
```

Lint a specific package:

```bash
PKG=0x.js yarn lint
```

### Run Tests

Run all tests:

```bash
yarn test
```

Run a specific package's test:

```bash
PKG=@0x/web3-wrapper yarn test
```

Run all contracts packages tests:

```bash
yarn test:contracts
```
### Deployed Contracts on Matic Mainnet

- transactionHash: 0x57a31bcc2331949f24ae9ede234e1f9e355939ad31169a6a8fa09cc5f752bc74
- ERC20Proxy successfully deployed at 0x66dc3b01f674b6c960cf60f3fb78e16342553cab
- transactionHash: 0x5e5c619a8363ffc4791ed3713605bdd77855bfee7999dc50ea6005fe2ad0626d
- ERC721Proxy successfully deployed at 0xb5d157ef45d8bfc9c413d00d0e902fe6a3ddbf8b
- transactionHash: 0x557f830a812aebe0b895b0bbaa20149e230908292ba5e359dfbaaf63f0bf38c4
- ZRXToken successfully deployed at 0x93719d8478d238c5996806a733e2068e0ead0b0e
- transactionHash: 0xd2cbb340a83af6591b7b0c84a15de098951d35bc263085755f49ea78f60e746b
- WETH9 successfully deployed at 0x6f3b2e10972cd42219f4108e72e9e15a616e5ba9
- transactionHash: 0x63e9a96faa111f0bbf48ae3df6f30f200d2f4281141d9ca4e740afcd1d249b45
- Exchange successfully deployed at 0x08330ac7b7f4a6695f41e3b8419113534cd61df0
- transactionHash: 0xfa15f97c9f45502bcf150a49aee02d78e2ac9298c55f19e3cc796e4e12b69a14
- DummyERC20Token successfully deployed at 0xc2c84b533a9518241e73d525afc89c3c57769e9f
- transactionHash: 0x8e13348198dd2c57d081c868a495bf3c4de04d5b090b01dd2e6b783ea57f8539
- DummyERC20Token successfully deployed at 0x48de9fa861a51ffe9fe0c614348d6e556034803b
- transactionHash: 0xcf7472860d84aa307b6f041c3234abc1d6d4ddc71c76e2d71a1dc01f83989465
- DummyERC20Token successfully deployed at 0x280c9ece1db286bea1c717849e0fc03bc38f7f8d
- transactionHash: 0xb1194bd8b4df51a1faeacb1019fdba4c083cf1871dd26f4877f2c4f3afa8d462
- DummyERC20Token successfully deployed at 0x20489f8affb46e30931a456fbbb4d92d9b655bf8
- transactionHash: 0x338b5d53a33c1b9a11425757c7881e6301b8cd11b19d3de91fa1d169e2f412ab
- DummyERC20Token successfully deployed at 0x46bf061ff7248cd33f060be98aa2fa57f0b9ce1f
- transactionHash: 0xa290bee10b323b67681c88609094638597a968e762a91669d916daa82be342d5
- DummyERC721Token successfully deployed at 0xbc5c7781f1e45c906195833a9a9967a19f175cc3
- transactionHash: 0x88c35b0bf25037b8d7ceac07abb574d929c4a9673a618707b9e6e5362aed6f50
- ERC1155Proxy successfully deployed at 0xade2af52f3dbe515e4abae89cfad06e6e60ff049
- transactionHash: 0x45c6b9ecfa956a91a134ead4e6d8e6a132ea7bd211d7e5179f46350c07f0d706
- StaticCallProxy successfully deployed at 0xc3bf2397eac18ff4107f6edf68e62aff1b11990d
- transactionHash: 0x1fffd16b406107fe58ca1e101acb10b73b91bfcaee6f12f0a0bfed095465ba55
- MultiAssetProxy successfully deployed at 0x636168180a78687127ee8479893f0a2f5eb7a640
- transactionHash: 0x6603f6e26dc904560efed8268599d2c85c02dd49c9ca7cfe05ade268e4b97666
- Forwarder successfully deployed at 0x995fde61633433fdb6d2c6f7ca885255d526f5c7
- transactionHash: 0xe737beb6a263e53970b2d43fbc6844bd39285f8c0d863520e78d73d4e69572b6
- OrderValidator successfully deployed at 0xab979e26f455465b094778b4717918e64d06c2dc
- transactionHash: 0xdcbb8223ba2dcf9825d6f2b3ef3e310973d56e4f5798c08e310025253c76a440
- DutchAuction successfully deployed at 0xb399ee7b4cb4344958bc47652b886c63493e3e42
- transactionHash: 0xf7937454959a68eee278d15537c4f58015ddb1ebe7a6d11960276f949fd1905d
- AssetProxyOwner successfully deployed at 0x8b8ebd096ed2ba7f415b5c185511eee8be59f814
- transactionHash: 0x01b82913dff28bcd2b2b66c099578d392cedfe9688e798008711500757352846
- CoordinatorRegistry successfully deployed at 0x9928a61ad210ae32e129d94195f27c556d33f963
- transactionHash: 0x315edcae37a834b0ea16644849659865cb6cd15d6f43d6583200ef44775094da
- Coordinator successfully deployed at 0x8b259a94e4b23816b2751c04dc03f9953ed91034
- transactionHash: 0xe43b7a87da062ce62a20579abb65ba73b18ada67c0ab0a4e001c4327c41c2cc9
- DevUtils successfully deployed at 0x35a6d26072d5b25c6dff261c756b0bf142e7c21b