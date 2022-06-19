# VueJS ~ IPFS

This package is intended to be used as a VueJS / IPFS boilerplate. You can directly upload the folder to [Pinata](https://www.pinata.cloud/) or [Web3.Storage](https://web3.storage) without adding any other step or complication.
Work as usual inside your VueJS website, then use the command `yarn deploy` to automatically deploy to IPFS.

First of all you need a `.env` file inside the folder `ipfs`, so you can copy the `.env.example` file adding your:
- `PINATA_KEY`: the JWT key generated by Pinata
- `PINATA_ENDPOINT`: the endpoint of your Pinata account
- `WEB3STORAGE_KEY`: the JWT generated by website
- `WEB3STORAGE_ENDPOINT`: you can leave it as `https://dweb.link/ipfs/` or customize if you want to use your own endpointt

Then you should be able to run the commands:
```
yarn deploy pinata
yarn deploy web3storage
```

Both will return a link like:
https://ipfs.yomi.digital/ipfs/QmaLoNrp3mwPq9WHvNL5GcJTsE5cNuNvGjzd1dZPs3ZFBg/#/
which will be the preview of your project.

## VueJS Project setup
```
yarn install
```

### VueJS hot-reloads for development
```
yarn serve
```