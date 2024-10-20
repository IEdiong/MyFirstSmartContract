# My First Smart Contract

## Part 1: Setting Up Your Development Environment

### Install MetaMask
MetaMask is an Ethereum wallet that allows you to manage your accounts, hold testnet ETH, and interact with smart contracts. Here’s how to get started:

1. **Visit the MetaMask Website:** Go to the MetaMask website and download the browser extension for your preferred browser (Chrome, Firefox, Brave, etc.).
2. **Create a Wallet:** After installing MetaMask, open it and follow the on-screen instructions to create a new wallet. Remember to store your seed phrase securely; this is your backup key for wallet recovery.
3. **Add Testnet ETH:** Within MetaMask, switch to a test network like Sepolia or Goerli. You can obtain free testnet ETH from a faucet, which will be used to deploy and interact with smart contracts without spending real ETH.

### Access Remix IDE
Remix is an online Integrated Development Environment (IDE) designed for Solidity smart contracts. It’s user-friendly and runs directly in your web browser.

1. **Open Remix:** Navigate to [Remix IDE](https://remix.ethereum.org/) in your browser. The interface includes a file explorer, code editor, and console.
2. **Create a New Workspace:** In the file explorer, create a new workspace to organize your projects. You can name it something like `MyFirstSmartContract`. This workspace will house all the files you’ll work on during your Solidity development. 

> *(The phrase “create a new workspace to organize your projects” was not helpful. I feel better descriptions of what to click to do certain things should have been well-detailed. Also, we should have been instructed to check the ‘initialize workspace as a new git repository’ checkbox seeing that we were going to later push the code to GitHub. After creating the new workspace, we should have been informed about what appears in the newly created workspace; referring to the ‘.prettierrc.json’ file.)*
3. **Create a Solidity File:** Inside your new workspace, create a new file with a `.sol` extension, such as `SimpleStorage.sol`. This is where you’ll write your first smart contract.

> *(After creating the file with the ‘.sol’ extension, we get a red squiggly line in the editor. A hint as to why this appears would have been helpful.)*


## Part 2: Writing My First Smart Contract
Now that your development environment is set up, let’s write your first smart contract.

1. **SPDX License Identifier:** Although not mandatory, it’s a good practice to start your contract with an SPDX License Identifier. This helps with code licensing and sharing.

```js
// SPDX-License-Identifier: MIT
```
2. **Compiler Directive:** Begin by specifying the pragma, which tells the compiler which version of Solidity to use. This ensures your contract is compiled with the correct version.

```js
pragma solidity ^0.8.25; // This allows any version from 0.8.25 to less than 0.9.0
```
3. **Write the Smart Contract:** Define your contract using the contract keyword, followed by the contract's name, like `SimpleStorage`. The code inside the curly brackets `{}` will define the behavior of your contract.

```js
contract SimpleStorage {
	uint256 public favoriteNumber; // State variable to store a number
}
```

## Part 3: Compile and Deploy the Contract Locally

### Compiling Your Contract

1. **Compile the Contract:** In Remix, select the Solidity Compiler from the sidebar.
Choose the Compiler Version: Ensure that the compiler version matches the one specified in your Solidity file.
2. **Click the Compile Button:** Compiling converts your human-readable code into machine-readable bytecode. If successful, you’ll see a green checkmark ✅. If there are errors, Remix will highlight them so you can fix them.

### Deploying Your Contract Locally

1. **Switch to Local Environment:** In Remix, go to the `"Deploy & Run Transactions"` tab. This is a local blockchain that runs in your browser.

> *(Use of inconsistent language, ‘Sidebar’, ‘Tab’)*
2. **Deploy the Contract:** Click the `"Deploy"` button. Remix will simulate deploying your contract to the local blockchain. This process doesn’t require MetaMask or real ETH.

3. **Interact with the Contract:** Once deployed, your contract will appear under `"Deployed Contracts"` in Remix. You can interact with the functions of your contract directly within the Remix interface.

> *(How do we interact with the contract? This part is unclear.)*

## Observations and Challenges

The comments in this file that look something like this
> *(Like this)*
are my observations and challenges. They were mostly solved by exploring the Remix IDE to discover things for myself.