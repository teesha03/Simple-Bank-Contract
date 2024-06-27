# Simple Bank Contract

## Description
This is a simple Ethereum contract that allows users to deposit, withdraw, and transfer funds. The contract also has a redeem function to reset the balance to 0.

## Getting Started


### Functions
- deposit(uint256 _amount): Deposits a specified amount of Ether into the contract.
- withdraw(uint256 _amount): Withdraws a specified amount of Ether from the contract.
- getBalance(): Returns the current balance of the contract.
- redeem(): Resets the balance of the contract to 0.
- transfer(address _to, uint256 _amount): Transfers a specified amount of Ether to a specified address.

### Executing program for frontend and smart contract
- Copy and paste the index.js, SmartContract.sol and deploy.js from the repository into your gitpod website.
- Remember index.js contains the frontend code.
- Open two additional terminals in your gitpod
- In the second terminal type: npx hardhat node
- In the third terminal, type: npx hardhat run --network localhost scripts/deploy.js
   Back in the first terminal, type npm run dev to launch the front-end.
After this, the project will be running on your localhost. Typically at http://localhost:3000/

### wallet setup
To interact with the smart contract, we need to set up a network with the MetaMask wallet.
- Click on the MetaMask extension and then click on the top right button -> settings.
- Click on "Add a Network."
- Click on "Add a Network Manually."
- Give the Network name (whatever you want).
- Set the New RPC URL to http:https://8545-metacrafterc-scmstarter-kodhc8ve1v6.ws-us114.gitpod.io
- Set the Chain ID to 31337.
- Set the Currency symbol.
Now, set the MetaMask wallet network to the newly created network.

To set up an account, you have to import the account's private key, which you can find in the second terminal where we executed the command npx hardhat node. After that, you can see there are many account numbers with private keys written in the terminal.Take any account's private key to import it to your Metamask Wallet.And Now your imported account is coonect to our METAMASK wallet and hence we can transfer our ethers.

Now open http://localhost:3000/ again and now you can interact with your frontend and METAMASK wallet and transfer tokens accordingly.

## License

This project is licensed under the MIT License - see the LICENSE.md file for details
