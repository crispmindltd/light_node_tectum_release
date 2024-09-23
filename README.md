# Welcome to Tectum Light Node v0.9! #

## Description ##

The Light Node is a component of the Tectum blockchain, designed to provide simplified access to the functionality of the blockchain network. It is developed for user convenience, without requiring full synchronization of the entire blockchain.

Main functions of the Light Node:
1. Token management.
2. Transaction processing.
3. User key management.
4. Interaction with the main network and other system components.

## Web Server ##
The Light Node also includes a local web server that processes these requests and interacts with other system components, such as WalletAPI.
It provides explorer functionality, allowing users to view information about blocks and transactions, as well as an interface for creating new tokens, making transfers, and managing keys.

## Endpoints ##

The Light Node supports the following types of requests:

## Requests Description ##

### Token operations: ###

-   GET /tokens: Retrieve a list of all tokens
-   POST /tokens: Create a new token
-   GET /tokens/fee: Retrieve fee of creating token
-   GET /tokens/ticker: Retrieve information about a specific token
-   POST /tokens/transfer: Transfer tokens
-   GET /tokens/transfer/fee: Retrieve fee of token transfer
-   GET /tokens/transfers: Retrieve token transfer history
-   GET /tokens/address/byid: Retrieve the smart contract address by ID
-   GET /tokens/address/byticker: Retrieve the smart contract address by ticker
-   GET /tokens/balance/byaddress: Retrieve token balance by address
-   GET /tokens/balance/byticker: Retrieve token balance by ticker

### TET operations: ###

-   GET /coins/balances: Retrieve balances for multiple tokens
-   POST /coins/transfer: Transfer TET
-   GET /coins/transfers: Retrieve TET transfer history
-   GET /coins/transfers/user: Retrieve TET transfer history for user
-   GET /coins/transfers/fee: Retrieve fee for transfer

### User management: ###

-   POST /user/auth: User authentication
-   POST /user/registration: Register a new user

### Key management: ###

-   POST /keys/generate: Generate new keys
-   POST /keys/recover: Recover keys using a seed phrase
-   GET /keys/public/byuserid: Retrieve the public key by user ID
-   GET /keys/public/byskey: Retrieve the public key by session key

### Blocks: ###

-   GET /blockscount: Retrieve count of blocks

## Launch ##
To start testing Tectum blockchain, you need to run the Tectum Lite file Node.exe. During startup, a reaction from the antivirus / firewall is possible, this is due to the features of the software, it is necessary to ignore the warning and continue the launch. We do NOT DISTRIBUTE malware, and you can be sure of the security of the application being launched.
After launching the application, you will be asked to enter your login details or register. When using it for the first time, click the "registration" button and fill in the required fields. The account is activated instantly!
The Light Node is designed with the necessity of ensuring the security of user data, including the use of session keys and encryption of sensitive information.

