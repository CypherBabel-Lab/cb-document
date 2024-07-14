# July

## BitoBridge  (5 July 2024)

### Features

* Complete the gas deduction module to process the transaction fee before the gas and protocol fees.
* Notification about the faucet claim's results.
* Add slippage for the gas fee of the target chain in the ICRC => ERC20 feature.
* Button for updating assets' balance.

### Optimizations

* Modify router canister to cope with updated gas rules. &#x20;
* Optimize UI for mobile display.
* Optimize UE and UI for the confirmation of bridging.
* Add skeleton loading to the fee area.

### Bugs

* Fix the stuck of subsequent unwraps caused by insufficient unwrap.
* Fix the encoding/decoding of the Bitcoin address in the Ethereum smart contract.
* Fix the stuck transaction on Ethereum caused by the bounce order.

## BitoBridge  (12 July 2024)

### Features

* Primary functions of the Statistics canister.
* The bridging histories of BTC and ICRC tokens.
* Integrate the Arbitrium testnet.
* Deploy the testnet on IC.

### Optimizations

* Upgrade the UI for the fee area.
* Notification when claiming testBITO without logging in.
* Reorganize the repositories as a Monorepo.

### Tests

* BTC bridging tests.
* ICRC bridging tests.
* BITO faucet tests.
