# 🗃 React dApp
This repository show you how to use **dApp** to connect to your wallet, call a function in smart contract with MetaMask and Web3 tools.

I have another repository to describe how to deploy a smart contract **[here](https://github.com/Justinianus2001/first-smart-contract)** and can use to interact in this project, or you can keep my smart contract information as sample.
## Setup
To interact with this project, we need the following tool: **[MetaMask](https://metamask.io/download/)** and **[Alchemy](https://auth.alchemyapi.io/signup)**.

With MetaMask, you need Goerli ETH to use as gas for call function, get free from a *[Goerli faucet](https://goerlifaucet.com/)*.

You also need an Alchemy app in Goerli network, after that create an *.env* file and fill this information:
```
REACT_APP_ALCHEMY_KEY = wss://eth-goerli.g.alchemy.com/v2/your-api-key
```
* Optional: Change smart contract will interact in this project.

Change two input value of two variables contractABI, contractAddress in *interact.js* with your smart contract ABI & address.
```
const contractABI = require("../contract-abi.json") // change in contract-abi.json;
const contractAddress = "your-contract-address";
```
## Execute
Install package and run React project
```
npm install
```
```
npm start
```