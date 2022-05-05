# Trakon SDK

Stage your hardhat and truffle compiled smart contracts with [Trakon](https://trakon.xyz). Then review, share, and deploy them from a [private dashboard](https://trakon.xyz/compilations).

![stage example in terminal](/docs/stage-example.gif)

## Installation

### Prerequisites

Trakon requires [node 16.x](https://nodejs.org/en/download/) and contracts to be compiled in a [Hardhat](https://hardhat.org/) or [Truffle](https://trufflesuite.com/) project
before staging.

#### Yarn 2

```shell
yarn dlx @zepheruslabs/trakon-sdk stage
```

#### Yarn

```shell
yarn global add @zepheruslabs/trakon-sdk
```

#### NPM

```shell
npm -g -i @zepheruslabs/trakon-sdk
```

## Usage

### Compile

In a Hardhat or Truffle project, compile your contracts using the framework's respective compile command.

#### Hardhat

```shell
npx hardhat compile
```

#### Truffle

```shell
truffle compile
```

### Stage

With the compiled contracts, you can run the Trakon `stage` command in the same project.

#### Yarn 2

```shell
yarn dlx @zepheruslabs/trakon-sdk stage
```

#### Yarn or NPM

```shell
trakon stage
```

Trakon will search in your local project for any compiled contracts and present a list of
found contracts ready to be staged. Select a contract to stage. Once the selected contract has
successfully been staged, you will be presented with a claimable link that you can share or
use for secure deployments.
