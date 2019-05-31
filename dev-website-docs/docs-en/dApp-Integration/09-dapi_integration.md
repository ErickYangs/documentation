
# DApp Integration Instructions

This series of access documents mainly introduces how dApp calls DAPI in various scenarios to implement operations such as login and calling smart contract.

Unlike traditional apps, dApp does not have a centralized account management backend, and users have full control over their identities and assets. As a result, DApps need to interact with blockchains in various ways, in addition to building their own business logic through smart contracts. In order to reduce the difficulty of DApp development, we provide a variety of DAPIs or methods for dApp and blockchain interaction, suitable for scenarios where dApp is used in all current mainstream devices.

The following scenarios are currently supported:

- [Use chrome plugin wallet](https://dev-docs.ont.io/#/docs-en/dApp-Integration/03-DAppDocking-use-chrome-extension-wallet)
- [Open DApp in mobile wallet](https://dev-docs.ont.io/#/docs-en/dApp-Integration/01-DAppDocking-Wallet-Opens-DApp)
- [Use mobile wallet to scan code](https://dev-docs.ont.io/#/docs-en/dApp-Integration/02-DAppDocking-QRcode)
- [Wake up mobile wallet](https://dev-docs.ont.io/#/docs-en/dApp-Integration/06-DAppDocking-Wake-up)


For the integration of DAPI-enabled wallets such as [ONTO](http://onto.app/) and [Math Wallet](http://www.mathwallet.org/en/), please refer to the corresponding integration documents. For details of the protocol, please see [CEP1](https://github.com/ontio-cyano/CEPs/blob/master/CEPS/CEP1.mediawiki).

Demo wallet download address: http://101.132.193.149/files/app-debug.apk

## Try dApps in Wallet

Mobile version Cyano wallet source link address：[cyano-android](https://github.com/ontio-cyano/cyano-android),[cyano-ios](https://github.com/ontio-cyano/cyano-ios).

H5 dApp example source code: [mobile-dapp-demo](https://github.com/ontio-cyano/mobile-dapp-demo).


### Open dApp in the wallet

Open dApp in the wallet：http://101.132.193.149:5000/#/

<div align="center">
  <img src="https://raw.githubusercontent.com/ontio-cyano/integration-docs/master/images/ios/01-dapps.jpg" height="350" width="200">
  <img src="https://raw.githubusercontent.com/ontio-cyano/integration-docs/master/images/ios/01-private-dapp.jpg" height="350" width="200">
  <img src="https://raw.githubusercontent.com/ontio-cyano/integration-docs/master/images/ios/01-open-dapp.png" height="350" width="200">
</div>

### Get account or identity information

If user identity verification is not required, dApp will directly query the account or identity information.

<div align="center">
  <img src="https://raw.githubusercontent.com/ontio-cyano/integration-docs/master/images/ios/01-open-dapp.png" height="350" width="200">
  <img src="https://raw.githubusercontent.com/ontio-cyano/integration-docs/master/images/ios/02-getAccount.jpg" height="350" width="200">
</div>

### dApp Login

If user identity verification is required, the dApp will send a signed message to the wallet and then verify the signature.

<div align="center">
  <img src="https://raw.githubusercontent.com/ontio-cyano/integration-docs/master/images/ios/01-open-dapp.png" height="350" width="200">
  <img src="https://raw.githubusercontent.com/ontio-cyano/integration-docs/master/images/ios/03-login-pwd.png" height="350" width="200">
  <img src="https://raw.githubusercontent.com/ontio-cyano/integration-docs/master/images/ios/04-logined.jpg" height="350" width="200">
</div>

### dApp Invoke SC

The calling contract process is:

1. Pre-execute contract after user signature
2. The user confirms and sends the transaction
3. Return the transaction hash to dApp

<div align="center">
  <img src="https://raw.githubusercontent.com/ontio-cyano/integration-docs/master/images/ios/input-password.jpg" height="350" width="200">
  <img src="https://raw.githubusercontent.com/ontio-cyano/integration-docs/master/images/ios/05-pre-exec-result.png" height="350" width="200">
  <img src="https://raw.githubusercontent.com/ontio-cyano/integration-docs/master/images/ios/06-dapp-recv-txhash.jpg" height="350" width="200">
</div>
