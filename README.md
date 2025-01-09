# Welcome to Tectum Light Node v1.0! #

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

### Token operations: ###

-   **[GET /tokens](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/tokens_list_request.md)**: Retrieve a list of all tokens with detailed information such as owner, name, ticker, amount, and more
-   **[POST /tokens](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/create_token_request.md)**: Create a new token
-   **[GET /tokens/fee](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/token_fee_request.md)**: Retrieve fee of creating token
-   **[POST /tokens/transfer](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/create_token_request.md)**: To transfer tokens between two addresses
-   **[GET /tokens/transfers](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/token_transfer_history.md)**: Retrieve the transfer history for a specific token
-   **[GET /tokens/transfer/fee](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/token_transfer_fee_v2.md)**: Retrieve the fee required for transferring a token
-   **[GET /tokens/address/byid](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/smart_contract_address_request.md)**: Retrieve the smart contract address by ID
-   **[GET /tokens/address/byticker](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/smart_contract_address_ticker_request.md)**: Retrieve the smart contract address by ticker
-   **[GET /tokens/balance/byaddress](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/token_balance_request.md)**: Retrieve token balance by address
-   **[GET /tokens/balance/byticker](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/token_balance_ticker_request.md)**: Retrieve token balance by ticker

### TET operations: ###

-   **[GET /coins/balances](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/docs/tet_coin_balance_request.md)**: Retrieve balances for multiple tokens
-   **[POST /coins/transfer](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/docs/tet_transfer_request.md)**: Transfer TET coins from one wallet to another
-   **[GET /coins/transfer/fee](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/docs/coin_transfer_fee.md)**: Retrieve the fee required for a coin transfer transaction
-   **[GET /coins/transfers](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/docs/coin_transfer_transactions.md)**: Retrieve TET transfer history
-   **[GET /coins/transfers/user](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/docs/tet_transfer_history_user.md)**: Retrieve the TET transfer history for a specific user

### User management: ###

-   **[POST /user/auth](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/user_authentication_request.md)**: Authenticate an existing user with their login and password
-   **[POST /user/registration](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/user_registration_request.md)**: To register a new user in the system.

### Key management: ###

-   **[POST /keys/recover](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/keys_recovery_request.md)**: Recover keys using a seed phrase
-   **[GET /keys/public/byuserid](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/public_key_by_userid_request.md)**: Retrieve the public key by user ID
-   **[GET /keys/public/byskey](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/public_key_by_skey_request.md)**: Retrieve the public key by session key

### Blocks: ###

-   **[GET /blockscount](https://github.com/crispmindltd/light_node_tectum/tree/main/docs/block_count.md)**: Retrieve the total count of blocks in the blockchain

**Launch**
To start testing Tectum blockchain, you need to run the Tectum Lite file Node.exe. During startup, a reaction from the antivirus / firewall is possible, this is due to the features of the software, it is necessary to ignore the warning and continue the launch. We do NOT DISTRIBUTE malware, and you can be sure of the security of the application being launched. After launching the application, you will be asked to enter your login details or register. When using it for the first time, click the "registration" button and fill in the required fields. The account is activated instantly! The Light Node is designed with the necessity of ensuring the security of user data, including the use of session keys and encryption of sensitive information.

**Usage of the Light node:**
- **The "Node" window:** This window displays blockchain events in real time.
- **The "Briefcase" window:** In this window, you can perform all the basic actions with the system using TET test tokens. In the "Make transaction" section, click the "Refresh" button to get a list of tokens available for transactions. Click on the token in the list in the "My tokens" window on the right side of the interface in the "Transfer" window, you will see your TET address. You can share this address with another member to have them transfer TET Test tokens to your account. You can also transfer TET from your wallet to any Test participant. In the "Token" section, you can get information about the ICO of the used token by entering the ICO number from the "My tokens" window of the "Make transaction" section in the "Token ID" field. The "Blocks" section displays information about the specified range of blockchain blocks (you can set a range of no more than 10 blocks). The Latest block section displays comprehensive information about the latest block range, including transaction speed, hash rate, and other block write parameters. The "Report" section displays information about the last 10 transactions between network members.

