# MyToken Project
MyToken is a basic ERC-20 compatible token smart contract written in Solidity. It includes functionality for minting and burning tokens, allowing for the creation and destruction of tokens while ensuring balance consistency.

## Description
 This project demonstrates fundamental Solidity concepts such as public variables, mappings, and functions, and can be used in various Ethereum-based applications.

## Getting Started

### Installing

* How/where to download your program:
  - Clone the repository:
    ```sh
    git clone https://github.com/yourusername/MyToken.git
    cd MyToken
    ```
* Any modifications needed to be made to files/folders:
  - Ensure you have the correct Solidity version specified in the `truffle-config.js` file:
    ```javascript
    compilers: {
      solc: {
        version: "0.8.18"
      }
    }
    ```

### Executing Program

* How to run the program:
  1. **Install Dependencies:**
     ```sh
     npm install
     ```
  2. **Start Ganache:**
     - Open Ganache and create a new workspace or quickstart a new Ethereum network.
  3. **Compile the Contract:**
     ```sh
     truffle compile
     ```
  4. **Deploy the Contract:**
     ```sh
     truffle migrate
     ```
  5. **Interact with the Contract:**
     - You can interact with the deployed contract using Truffle console:
     ```sh
     truffle console
     ```
     Inside the console:
     ```javascript
     let instance = await MyToken.deployed()
     let accounts = await web3.eth.getAccounts()

     // Mint tokens
     await instance.mint(accounts[1], 1000)

     // Burn tokens
     await instance.burn(accounts[1], 500)
     ```

## Help

Any advice for common problems or issues.
```sh
truffle help
```
## Authors

Contributors names and contact info

Inderpreet Singh  
indersingh46334@gmail.com


## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
