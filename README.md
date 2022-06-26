# Decentralized Land Registration

Blockchain based Land Registration and transfer of entitlement system where the land ownership and all its details are stored in the Blockchain with zero chances of forgery in ownership.

## Challenges we faced
The main issue we encountered was figuring out how to integrate the truffle environment, which handles all of the blockchain-related backend, with the front-end react app. To interact with the smart contract via the front end, we used Web3.js. However, the documentation on Web3.js was insufficient for our needs. We were able to bridge the gap and make the app run smoothly with the help of some helpful blogs.
There were some difficulties in connecting Metamask to the local Ethereum network that we built. It took some time, but with the help of useful documentation from metamask, we were able to integrate the metamask authentication.

Tools used:
1. React.js used for front-end development.
2. Solidity used for back-end development.
3. Truffle and Web3.js
4. Ganache used as a local blockchain.
5. Metamask wallet.

This README file directs you how to install this project and the various dependencies on your local system and run this project locally. Before proceeding to clone, amke sure you have node@16.14.0 and greater installed in your local system.

Cloning and dependencies
Clone this repository in your local system by running the following command in your preferable terminal.

git clone https://github.com/emharsha1812/Land-Registry-Hackathon.git
After cloning the repository, move into the directory by the following command

cd Land-Registry-Hackathon 
Install the various dependencies required for the project to work by running

npm install  
Install truffle and ganache-cli

truffle v5.2.4
ganache-cli v6.12.2

npm install -g truffle
npm install -g ganache-cli
Deploy contratcs and run locally
Install metamask browser extension Download and install metamask from here. Before proceeding further, it is advisable to split 3 terminals to avoid confusion. Run local Ethereum blockchain on first terminal

ganache-cli
> Note: Do not close `ganache-cli` (the blockchain network needs to be running all the time)
Configure metamask on the browser with following details

New RPC URL: http://localhost:8545
Chain ID: 1337 Import accounts using private keys from ganache-cli to the metamask extension on the browser

Run client side
Deploy smart contract to the (local) blockchain

# on the Election-blockchain-class directory
truffle migrate
Note: Use truffle migrate --reset for re-deployments

Launch the development server (fronted)

npm start
Note: If you face text visibility errors on client side, try changing your browser to dark mode.

