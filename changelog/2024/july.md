# July

## BitoBridge  (5 July 2024)

### Features/Functions

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

