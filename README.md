# NanoVault

NanoVault is a fully client-side signing wallet for sending and receiving [Nano](https://github.com/nanocurrency/raiblocks) 
on your [desktop](https://github.com/valnexo/nanovault/releases) or [in your browser](https://nano-vault.io)

![NanoVault Screenshot](https://s3-us-west-2.amazonaws.com/nanovault.io/NanoVault-Preview.png)
___

# Table of Contents
* [Install](#install-nanovault)
* [Bugs/Feedback](#bugsfeedback)
* [Application Structure](#application-structure)
* [Development Prerequisites](#development-prerequisites)
* [Development Guide](#development-guide)
* [Acknowledgements](#acknowledgements)


# Install NanoVault
NanoVault is available on your desktop (Windows/Mac/Linux) - just head over to the [releases section](https://github.com/valnexo/nanovault/releases) and download the latest version for your OS.

You can also use NanoVault from any device on the web at [nano-vault.io](https://nano-vault.io)


# Bugs/Feedback
If you run into any issues, please use the [GitHub Issue Tracker](https://github.com/valnexo/nanovault/issues).

___

#### Everything below is only for contributing to the development of NanoVault
#### To download NanoVault go to the [releases section](https://github.com/valnexo/nanovault/releases), or use the web wallet at [nano-vault.io](https://nano-vault.io)

___

# Application Structure

NanoVault is a client-side wallet application providing the user interface, seed generation, block signing, and related wallet functionality.


# Development Prerequisites
- Node Package Manager: [Install NPM](https://www.npmjs.com/get-npm)
- Angular CLI: `npm install -g @angular/cli`


# Development Guide
#### Clone repository and install dependencies
```bash
git clone https://github.com/valnexo/nanovault
cd nanovault
npm install
```

#### Run the wallet in dev mode
```bash
npm run wallet:dev
```

## Build Wallet (For Production)
Build a production version of the wallet for web:
```bash
npm run wallet:build
```

Build a production version of the wallet for desktop: *(Required for all desktop builds)*
```bash
npm run wallet:build-desktop
```

## Desktop Builds

*All desktop builds require that you have built a desktop version of the wallet before running!*

Run the desktop wallet in dev mode:
```bash
npm run desktop:dev
```

Build the desktop wallet for your local OS (Will be in `dist-desktop`):
```bash
npm run desktop:local
```

Build the desktop wallet for Windows+Mac+Linux (May require dependencies for your OS [View them here](https://www.electron.build/multi-platform-build)):
```bash
npm run desktop:full
```

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

# Acknowledgements
Special thanks to the following!
- [numtel/nano-webgl-pow](https://github.com/numtel/nano-webgl-pow) - WebGL PoW Implementation
- [jaimehgb/RaiBlocksWebAssemblyPoW](https://github.com/jaimehgb/RaiBlocksWebAssemblyPoW) - CPU PoW Implementation
- [dcposch/blakejs](https://github.com/dcposch/blakejs) - Blake2b Implementation
- [dchest/tweetnacl-js](https://github.com/dchest/tweetnacl-js) - Cryptography Implementation

If you have found NanoVault useful and are feeling generous, you can donate at `xrb_318syypnqcgdouy3p3ekckwmnmmyk5z3dpyq48phzndrmmspyqdqjymoo8hj`
