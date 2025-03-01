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
