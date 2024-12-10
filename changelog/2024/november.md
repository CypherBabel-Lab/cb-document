# November

## BitoBridge  (1 November 2024)

### New Features

* **Sui Blockchain Integration**: Fully implemented support for bridging BTC and ICRC tokens to the Sui blockchain leveraging the tEd25519 signature.
* **Mainnet Launch**: Successfully launched on the mainnet, it now supports seamless interoperability between Bitcoin, ICP, Ethereum, Arbitrum, Polygon, and Sui blockchains. Users can now bridge assets across these networks with improved speed and security.

### Optimizations

* **User Interface Improvements**: Revamped the dashboard logic for a more intuitive user experience; Enhanced wallet integration features, allowing for easier management of multi-chain assets.

### Bug Fixes

* **Transaction Failure Resolution**: Fixed an issue where cross-chain transactions occasionally failed during network congestion periods.
* **Synchronization Error**: Resolved a bug causing delays in balance updates after completing a bridging transaction.
* **UI Glitches**: Corrected display issues on the transaction history page where some entries were not showing correctly; Fixed a problem where the network selection dropdown was unresponsive on certain browsers.

## BitoBridge  (8 November 2024)

### New Features

* **BNB Smart Chain Integration:** Support for BNB Smart Chain was added on both Testnet and Mainnet.

### Optimizations

* **Wallet Manager UX:** Improved user experience for switching between supported blockchains and wallets.

## BitoBridge  (15 November 2024)

### New Features

* **Base Blockchain Integration**: Integrated Base blockchain into both Testnet and Mainnet.

### Optimizations

* **History Table UI**: Enhanced the history table design for better data visibility and readability.

## BitoBridge  (22 November 2024)

### New Features

* **SNEED Token Support:** Enabled SNEED token on the Mainnet.
* **Bitget Wallet Integration:** Added support for Bitget wallet across EVM blockchains, Bitcoin, and Sui.
* **Additional Blockchain Integrations:**
  * Mainnet: Polygon and Arbitrum.
  * Testnet: Berachain.

### Optimizations

* **History Table UI:** Further optimized the history table for improved data presentation.&#x20;

### Bug Fixes

* **Sui Smart Contract:** Resolved an issue in the helper smart contract on Sui.

## BitoBridge  (29 November 2024)

### New Features

* **ICRC1 Token Standard Support:** Added support for the ICRC1 token standard, enhancing interoperability.
* **WindogeXP Token Support:** Enabled support for the WindogeXP token on the Mainnet, expanding token compatibility.
* **ICRC28 Support**: Integrated ICRC28 standard at the backend for improved functionality and future extensibility.
* **Additional Blockchain Integrations:**
  * Mainnet: Added support for Optimism.
  * Testnet: Integrated Optimism, enabling testing and development compatibility.

### Optimizations

* **Wallet Connection Logic:** Removed the requirement to connect an Internet Computer (IC) wallet to use the bridge, streamlining the user experience.
* **Wallet Manager Initialization**: Improved the initialization logic for the wallet manager, ensuring faster and more reliable wallet operations.

### Bug Fixes

* **Stable Memory Storage**: Modified some data to be stored in stable memory and provided a data migration API to address the issue of excessive instruction consumption during upgrades.
