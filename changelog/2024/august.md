# August

## BitoBridge  (2 August 2024)

### Features

* Add a supported blockchain: StratoVM.
* Add a supported ICRC token: ckTESTBTC.

### Optimizations

* Interactive buttons for all pages.
* Responsive UI.
* Replace the faucet claim's animation.
* Add a retry option for the order confirmation pop-up window.

### Bugs

* Fix the ordering of EVM to ICP bridging transactions.

## BitoBridge  (9 August 2024)

### Features

* Add two supported wallets: NFID and Bitfinity wallet.
* Core logics of V2.

### Optimizations

* Update the logic of the wallet manager to support better adding wallets.
* Update the ic0 URL to a customized URL.
* Optimize the frontend code structure for V2.



## BitoBridge  (16 August 2024)

### Features

* Develop relayer\_evm of BitoBridge V2.
* Develop frontend bridging logic of BitoBridge V2.
* Integrate ICP Bridge in BitoBridge V2.
* Integrate history records of transactions in BitoBridge V2.

### Optimizations

* Optimize the logic of the Hub to accommodate relayer\_evm.
* Newly designed UI for BitoBridge V2.

### Tests

* Through testing of canisters' core logics in BitoBridge V2.

##

## BitoBridge  (23 August 2024)

### Features

* Add fee logic in the Hub canister in V2.
* Add cache event in V2.
* Add a transaction details modal on the frontend in V2.
* Add a cache for claim history on the frontend in V2.
* Add relayer\_btc canister in V2.
* Support bridging between any two blockchains besides BTC in V2.
* Support bridging from Bitcoin blockchain to other blockchains in V2.

### Optimizations

* Optimize core logic in V2.
* Optimize the history table on the frontend in V2.
* Unify the pop-up window modal on the front end in V2.

### Tests

* Fee logic.
* Claim history.
* The core logic for bridging.



## BitoBridge  (30 August 2024)

### Features

* Support bridging from other blockchains to Bitcoin blockchain in V2.
* Add history filters for all transactions to the hub canister.
* Add a pause function to the hub canister.
* Add a unique logic for IC <=> Bitcoin blockchain bridging.
* Add a protocol fee ledger to the hub canister.
* Add a unique logic for IC <=> Bitcoin blockchain protocol\_fee.

### Optimizations

* Optimize mint\_proof's failure logic.
* Optimize relayer\_btc canister's transaction logic for simultaneous submissions to multiple blockchains.
* Optimize relayer\_btc canister's logic for processing a correct tx\_id after an incorrect tx\_id. &#x20;
* Optimize the logic for RPC node timeout. &#x20;

### Tests

* Core logic unit tests.
* User interaction simulation tests.
* Integration test.
