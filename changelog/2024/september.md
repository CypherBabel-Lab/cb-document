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

