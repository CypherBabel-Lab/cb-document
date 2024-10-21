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
