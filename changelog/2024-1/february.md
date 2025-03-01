# February

## 08 February 2025 - BitoIndexer Development Update

### Features

* Block Parser Enhancement: Added code to parse _ordinal inscription data_ in Bitcoin blocks, storing key attributes (timestamp, inscription size).
* Transaction Tagging: Implemented a rudimentary tagging system for _meta-protocol transactions_, allowing easy filtering of Runes vs. Ordinals.

### Updates

* Repo Restructuring: Moved all parsing logic under a dedicated parsers/ directory, making it easier to add new protocols in the future.
* Data Schema Adjustments: Slightly modified the database schema to include a metaType field in the transactions table.

### Bugs Fixed

* Block Height Mismatch: Resolved an off-by-one error causing newly mined blocks to be indexed as one height lower.

### Optimizations

* Caching: Added a small in-memory cache to reduce repeated decoding for frequently accessed meta-protocol transactions, improving average query speed by \~20%.
* Thread Pool Tuning: Adjusted thread pool settings to better handle parallel block parsing (reduced idle CPU overhead).

## 15 February 2025 - BitoIndexer Development Update
