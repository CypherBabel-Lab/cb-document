# October

## BitoBridge  (12 October 2024)

### New Features

* Initiation of Testnet Engagement Phase II.
* Faucet updated to provide a randomized amount of tokens.
* Deployment of a new TESTBITO token contract for Phase II.

### Optimizations

* Improved front-end code for better performance and user experience.
* When bridging fails, the system now displays a ‘retry’ button instead of ‘ok.’

### Bug Fixes

* Updated contract logs to use safe/finalized instead of latest to prevent inaccuracies.
* Removed unnecessary approval steps to avoid unintended remaining transaction fees.

## BitoBridge  (18 October 2024)

### New Features

* Integrate the Sui Wallet.
* Integrate the Xverse wallet.
* Integrate the Sui network, partially done.

### Optimizations

* Introduced a timeout mechanism for bridging operations.
* Adopted EIP-712 standardized message formats for improved security and interoperability.

### Bug Fixes

* Added security headers in HTTP responses and meta tags for enhanced protection.
* Implemented a guard to ensure events are marked as processed, even if a panic occurs after the hub call.

## BitoBridge  (25 October 2024)

### New Features

* Enabled bridging to the Sui network using the tSchnorr signature, with work in progress for bridging back from Sui.
* Preparations underway for the BitoBridge Mainnet launch.

### Optimizations

* Enhanced transaction validation logic to improve accuracy and reduce processing time.
* Optimized smart contract gas usage for bridging operations, minimizing fees for users.
* Improved UI responsiveness for better user experience across different devices and network conditions.

### Bug Fixes

* Resolved an issue where engagement points were being doubled during calculation, ensuring accurate user rewards.
* Fixed a bug causing transaction delays during peak times, improving overall bridging speed.
* Addressed a minor display issue in the wallet balance panel, ensuring accurate and real-time token balance updates for users.
