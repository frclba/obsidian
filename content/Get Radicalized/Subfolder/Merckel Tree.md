[[Blockchains]]

A Merkle tree (named after Ralph Merkle) is a data structure that lets you efficiently verify the integrity of large datasets. It's one of the foundational building blocks of blockchain technology.

How it works — think of it like a family tree, but for data:
- At the bottom, you have your actual data blocks (transactions, files, whatever)
- Each block gets hashed (a cryptographic fingerprint)
- Pairs of hashes are combined and hashed together to form a parent node
- This continues upward until you reach a single hash at the top: the **Merkle root**

The magic: if any single piece of data at the bottom changes (even by one bit), its hash changes, which changes its parent's hash, which cascades all the way up to the root. The root hash is a fingerprint of the *entire* dataset.

Why this is powerful:
- **Efficient verification** — to verify one transaction in a block of thousands, you don't need to download the whole block. You just need the transaction, plus a handful of hashes along the path to the root. This is called a "Merkle proof."
- **Tamper detection** — any modification to any data anywhere in the tree changes the root hash. This makes it trivially easy to detect tampering.
- **Blockchain integrity** — each block in a blockchain contains the Merkle root of all its transactions. This is how light clients can verify transactions without downloading the entire blockchain.

Merkle trees aren't just used in blockchains. They're used in Git (version control), certificate transparency, distributed file systems (IPFS), and database synchronization.

The concept is simple but the implications are profound: it lets you have trust in data integrity without needing to trust any single party.

Related: [[Blockchains]], [[Ethereum Smart Contract Security Best Practices]]
