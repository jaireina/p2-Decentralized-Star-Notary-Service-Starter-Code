# REQUESTED INFO

Note: This was deployed to Goerli since Rinkeby has been deprecated

- ERC-721 Token Name: UStar
- ERC-721 Token Symbol: USTR
- Version of Truffle: v5.4.22
- Version of OpenZeppelin used:2.3
- Token Address on the Goerli Network: 0x36a7A3f69b4AcAf3ced04b8BccdfeD98cFFfC7b9 / https://goerli.etherscan.io/address/0x36a7A3f69b4AcAf3ced04b8BccdfeD98cFFfC7b9

If you want to deploy the smart contract to Goerli using truffle, make sure to include a `.env` file at the root of the project with your metamask mnemonic, like this

```
METAMASK_MNEMONIC=your seed words here
```

# ND1309 C2 Ethereum Smart Contracts, Tokens and Dapps - Project Starter

**PROJECT: Decentralized Star Notary Service Project** - For this project, you will create a DApp by adding functionality with your smart contract and deploy it on the public testnet.


### Dependencies

For this project, you will need to have:

1. **Node and NPM** installed - NPM is distributed with [Node.js](https://www.npmjs.com/get-npm)

```bash
# Check Node version
node -v
# Check NPM version
npm -v
```

2. **Truffle v5.X.X** - A development framework for Ethereum.

```bash
# Unsinstall any previous version
npm uninstall -g truffle
# Install
npm install -g truffle
# Specify a particular version
npm install -g truffle@5.0.2
# Verify the version
truffle version
```

2. **Metamask: 5.3.1** - If you need to update Metamask just delete your Metamask extension and install it again.

3. [Ganache](https://www.trufflesuite.com/ganache) - Make sure that your Ganache and Truffle configuration file have the same port.

4. **Other mandatory packages**:

```bash
cd app
# install packages
npm install --save  openzeppelin-solidity@2.3
npm install --save  truffle-hdwallet-provider@1.0.17
npm install webpack-dev-server -g
npm install web3
```

### Run the application

1. Clean the frontend

```bash
cd app
# Remove the node_modules
# remove packages
rm -rf node_modules
# clean cache
npm cache clean
rm package-lock.json
# initialize npm (you can accept defaults)
npm init
# install all modules listed as dependencies in package.json
npm install
```

2. Start Truffle by running

```bash
# For starting the development console
truffle develop
# truffle console

# For compiling the contract, inside the development console, run:
compile

# For migrating the contract to the locally running Ethereum network, inside the development console
migrate --reset

# For running unit tests the contract, inside the development console, run:
test
```

3. Frontend - Once you are ready to start your frontend, run the following from the app folder:

```bash
cd app
npm run dev
```

---

### Important

When you will add a new Test Network in your Metamask client, you will have to provide:

| Network Name      | New RPC URL              | Chain ID |
| ----------------- | ------------------------ | -------- |
| Private Network 1 | `http://127.0.0.1:9545/` | 1337     |

The chain ID above can be fetched by:

```bash
cd app
node index.js
```