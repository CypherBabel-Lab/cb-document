# September

## BitoBridge  (6 September 2024)

### New Features

* **Resubmit Function**: Users can now reactivate their expired transactions, enhancing the transaction management process.
* **Notification Area**: A new notification section has been added to the webpage to keep users informed of updates and alerts.

### **Optimizations**

* **Extended BTC Bridging Transaction Validity**: The valid period for BTC bridging transactions has been extended, reducing the likelihood of transaction expiry.
* **Lost Event Removal**: The `lost_event` has been removed for cases where the Internet Computer (IC) is the target chain.
* **Improved Claiming Animation**: The animation for claiming transactions has been replaced for greater clarity and a more user-friendly experience.
* **Resubmit Function Support**: Backend canisters (hub and relayer\_btc) have been optimized to support the new resubmit functionality.
* **RPC Node Stabilization**: The RPC nodes used by the frontend have been replaced to improve stability and ensure smoother operations.
* **History Table Optimization**: The history table now updates automatically in the background for a more seamless user experience.

### **Bug Fixes**

* **Time Parsing Error**: The issue with incorrect time parsing in the history table has been resolved.
* **Rank Display Error**: Fixed the rank display issue in the campaign ranking table.
* **EVM Wallet Connection Issue**: Resolved the error where the history table was displayed without connecting an EVM wallet.
* **Plug Wallet Pop-up**: Fixed the issue where no pop-up window appeared when using the Plug wallet.
* **EVM Chain Bridging Signing Error**: Addressed the signing error that occurred when bridging between EVM chains.
* **Internet Identity Login Error**: Corrected the invalid login issue with Internet Identity.
* **Balance Loading Error**: Fixed the error where balance loading failed.

## BitoBridge  (13 September 2024)

### New Features

* **Transaction Link in Record Details**: Added direct links to transactions within record details for easier access and verification.
* **Display of tx\_id on Source Chain**: Implemented the display of transaction IDs (tx\_id) on the source chain to enhance transparency and tracking.&#x20;

### **Optimizations**

* **Frontend Cache Management**: Improved performance by promptly clearing the local cache on the frontend, ensuring users receive the most up-to-date information.
* **Stable Memory Usage in relayer\_evm Canister**: Updated the logic to save data to stable memory during canister upgrades and retrieve it afterward, preventing data loss and maintaining cache integrity.
* **Enhanced Log Retrieval in relayer\_evm Canister**: Added the ability to fetch eth\_logs for specified blocks, enabling recovery of user data in cases where data might be lost.
* **Optimized Cache Submission in relayer\_evm Canister**: Improved logic to stop submitting cache to the hub once it has been confirmed that the hub already possesses the cache, reducing unnecessary operations.
* **Primary Key Modification in relayer\_btc Canister**: Modified the primary key and implemented the “tx\_id + address” logic, aligning with the agreed-upon standards for better data management and security.

### **Bug Fixes**

* **Unisat Signing Rejection Handling**: Fixed error handling when Unisat signing is rejected, ensuring the system responds appropriately without crashing.
* **get\_histories Instruction Limit in Hub Canister**: Resolved the issue where the get\_histories function exceeded instruction limits, which was causing failures in retrieving user histories.
* **Campaign Points Synchronization Error**: Corrected the error in campaign points calculation caused by the sync\_histories instruction limit, ensuring accurate point tracking.
* **Invalid Resubmission in relayer\_btc Canister**: Fixed the issue where invalid resubmissions were allowed, enhancing the integrity of transaction processing.

## BitoBridge  (20 September 2024)

### New Features

• **Blockchain Integration**: Added support for the Polygon Amoy Testnet.

• **Point Parameter Update**: Set a new credit factor of 3 for the Polygon Amoy Testnet as part of the Testnet Engagement Campaign.

• **BITOP Contracts**: Ongoing development and testing of BITOP contracts on both ICP and Polygon networks.
