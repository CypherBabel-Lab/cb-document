# February

## 08 February 2025 - BitoIndexer Development

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

## 15 February 2025 - BitoIndexer Development

### Features

* Expanded Protocol Coverage: Added initial support for an _experimental token protocol_, allowing BitoIndexer to recognize custom tokens minted on Bitcoin via advanced scripts.
* Search API: Exposed a /search endpoint for public queries, returning transaction data by block range or address.

### Updates

* Documentation: Updated our README.md and wiki pages to outline the new search endpoint and how to configure advanced token parsing.
* Continuous Integration (CI): Set up automated builds and basic unit tests running on each pull request to ensure stable merges.

### Bugs Fixed

* High Memory Usage: Identified and fixed a memory leak in the block processing loop where transaction buffers weren’t freed after parsing.
* Incorrect Timestamp Conversion: Corrected an error that displayed block timestamps in UTC+0 but labeled them incorrectly as local time.

### Optimizations

* Index Write Efficiency: Batched writes to the underlying database, cutting overall block parsing time by around 25%.
* Incremental Sync Mode: Implemented a partial sync mode, allowing newly joined nodes to index from the latest block backward without reprocessing the entire chain.

## 22 February 2025 - BitoIndexer Development

### Features

* Meta-Protocol Decoder API: Created an extensible decoder interface that third-party developers can implement to add new Bitcoin meta-protocols without modifying core code.
* Event Logging: Introduced an event log for each parsed transaction, which can be visualized in a dashboard (still in early alpha).

### Updates

* Build Pipeline: Extended CI checks to include integration tests that validate end-to-end indexing of small sets of blocks from regtest.
* Node Clustering: Began designing a clustering mechanism where multiple BitoIndexer nodes can share an index state, preventing duplication of parsing work.

### Bugs Fixed

* Address Parsing Anomaly: Fixed an issue where certain addresses with unusual script patterns weren’t recognized by the parser, leading to partial data.
* Rare Race Condition: Addressed a synchronization bug causing random index corruption when multiple threads tried writing to the DB simultaneously.

### Optimizations

* Thread-Safe Queues: Rewrote the internal queue system to reduce lock contention, boosting throughput for high-volume block syncs.
* Pruned Node Compatibility: Fine-tuned the code to work seamlessly with pruned Bitcoin nodes, saving disk space for smaller operators.
