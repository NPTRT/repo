[[Mempool]] or memory pool refers to a backlog of pending and unconfirmed transactions in a blockchain.

These unconfirmed transactions wait in the mempool to get validated and finalized in the upcoming block.

When you transact on a blockchain network, your crypto payments or transfers are not immediately confirmed. Your transactions have to be validated by miners on proof-of-work (PoW) blockchains and by validators on proof-of-stake (PoS) blockchains, who compile pending transactions into blocks.

Your transactions are only considered final once it is included in a block. Until then, your transactions will wait in a queue alongside all the other unconfirmed transactions in a place called the mempool.

The time taken to finalize a transaction will depend on the following factors:

- Blockchain network
- Time between blocks
- Gas fee
- Network congestion

The journey of a transaction from initiation to confirmation involves several steps. When a transaction is executed on a blockchain, it is broadcast to the entire network and queued in a mempool.

It is important to note that mempools are not standardized. Each blockchain node has its own mempool with transactions that may or may not differ from the transactions in a mempool of another node. A node may be configured in a way to receive transactions at different times, while some nodes may use lower-end hardware which can limit the amount of transactions it can store in its mempool.

Another important fact about the mempool is that not all the transactions in a mempool are treated equally. A miner or validator has the discretion to choose and pick which transactions to prioritize when creating a block.

Users often pay higher-than-average gas fees and offer tips to incentivize miners and validators to prioritize their transactions. Miners and validators are always looking to extract the maximum value ([[Maximal extractable value (MEV)]]) from a block due to the limited blockspace.