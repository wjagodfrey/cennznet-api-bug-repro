Reproduces a simple error when installing and requiring `@cennznet/api`

## Solution
Use `yarn add @cennznet/api` instead of `npm install --save @cennznet/api` as recommended by the `@cennznet/api` README.

Have asked the CENNZnet team to update the README.

## Problem
On running the example errors similar to the following are printed:
```
@polkadot/wasm-crypto has multiple versions, ensure that there is only one installed.
Either remove and explicitly install matching versions or deupe using your package manager.
The following conflicting packages were found:
        3.2.4   /---/cennznet-api-bug-repro/node_modules/@polkadot/keyring/node_modules/@polkadot/wasm-crypto
        3.2.4   /---/cennznet-api-bug-repro/node_modules/@polkadot/metadata/node_modules/@polkadot/wasm-crypto
        3.2.4   /---/cennznet-api-bug-repro/node_modules/@polkadot/types/node_modules/@polkadot/wasm-crypto
        3.2.4   /---/cennznet-api-bug-repro/node_modules/@polkadot/api/node_modules/@polkadot/wasm-crypto
@polkadot/util-crypto has multiple versions, ensure that there is only one installed.
Either remove and explicitly install matching versions or deupe using your package manager.
The following conflicting packages were found:
        5.9.2   /---/cennznet-api-bug-repro/node_modules/@polkadot/keyring/node_modules/@polkadot/util-crypto
        5.9.2   /---/cennznet-api-bug-repro/node_modules/@polkadot/metadata/node_modules/@polkadot/util-crypto
        5.9.2   /---/cennznet-api-bug-repro/node_modules/@polkadot/types/node_modules/@polkadot/util-crypto
        5.9.2   /---/cennznet-api-bug-repro/node_modules/@polkadot/api/node_modules/@polkadot/util-crypto
```

## Install
```
npm i
```

## Run
```
node index.js
```