# HAECHI-CLI (haechi-cli) 

[![CircleCI](https://circleci.com/gh/HAECHI-LABS/haechi-cli.svg?style=svg)](https://circleci.com/gh/HAECHI-LABS/haechi-cli)[![Coverage Status](https://coveralls.io/repos/github/HAECHI-LABS/HAECHI-CLI/badge.svg?branch=master)](https://coveralls.io/github/HAECHI-LABS/HAECHI-CLI?branch=dev)
[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org)

> Command Line Interface for the upgradeable smart contract framework. 

HAECHI-CLI is a new Command Line Interface tool created to help developers easily develop better DApps by providing an upgradeable smart contract framework as well as new development tools.

Upgradeable Smart Contract helps to easily fix bugs and update business logics for the Dapp service.
It also provides a high-quality user experience while maintaining the same entry point for users and updating smart contracts atomically.

It helps to develop, upgrade, test, compile and control the user’s current version of the Dapp service.

If you want more information about the Upgradeable Smart Contract Framework, you can take a look at the HAECHI-LABS [pdf file](https://drive.google.com/file/d/1xbvd3TeuOPXbMcDs-RhEFdqwxhLNXtNC/view?usp=sharing).

| **Contributors**: Please see the [Contributing](#contributing) section of this README. |
| --- |

## Table of Contents

- [Install](#install)
- [Usage](#usage)
- [Commands](#commands)
- [Contributing](#contributing)
- [Contact](#contact)
- [License](#license)

## Install

Install [Node.js](http://nodejs.org/) first.
Then, install [npm](https://npmjs.com/) and
```sh
$ npm install --global @haechi-labs/haechi-cli
```
or install [yarn](https://yarnpkg.com) and
```sh
$ yarn global add @haechi-labs/haechi-cli
```

## Usage

For a default set of files, run the following within an empty project directory:
```sh
$ mkdir my-project
$ cd my-project
$ haechi init
```
You don't have to do `` $ npm init `` or ``$ truffle init``.
We supports environment for [truffle](https://truffleframework.com/truffle).

_[See details](./commands/README.md#init)_ for ``$ haechi init``.

Then, install node modules according to ``package.json``.
```sh
$ npm install
```
or
```sh
$ yarn install
```

We recommend to use [ganache](https://truffleframework.com/ganache) for test.

Next, you have to write:

 - ``.env`` : General settings for your project 
 - ``service.haechi.json`` : Settings for your Dapp service
 
Please see [CONFIGURATION.md](./CONFIGURATION.md) to configure your project.

Run `$ haechi --help` for more details about functions of haechi-cli.

## Commands

Please see linked documentation below:
- [init](./commands/README.md#init): Initialize project directory
- [compile](./commands/README.md#compile): Compile solidity contract files
- [deploy-contract](./commands/README.md#deploy-contract): Deploy contract
- [deploy-service](./commands/README.md#deploy-service): Deploy service according to Upgradeable Smart Contract Framework
- [abi-to-script](./commands/README.md#abi-to-script): Generate javascript APIs interacting with smart contract on blockchain
- [flatten](./commands/README.md#flatten): Flatten several contract files in one file

## Contributing

Thank you for considering to join this project! We always welcome contributors :)

*Notes on project main branches:*
- `master`: Stable, released version
- `dev`: Work targeting stable release

To contribute, please see [CONTRIBUTING.md](./CONTRIBUTING.md).

## Contact 

- General Contact: hello@haechi.io
- [Facebook](https://www.facebook.com/HAECHILABS/)
- [Medium](https://medium.com/haechi-labs)

## License

MIT
