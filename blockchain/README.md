# Blockchain — A Beginner’s Guide

A **Blockchain** is a type of **Distributed Ledger Technology (DLT)** that consists of a growing list of records, called **blocks**, securely linked together using **cryptography**.

---

## Key Concepts

- **Distributed Ledger Technology (DLT)**
- **Blocks**
- **Cryptography**

---

##  Distributed Ledger Technology (DLT)

A **ledger** is a record book that keeps track of transactions.  
In traditional systems, ledgers are stored in **centralized databases**—meaning one authority controls the data.

In contrast, **blockchain** is a **distributed ledger**, meaning every participant (or *node*) in the network holds a copy of the same ledger.  

### Centralized vs. Distributed Example

**Centralized Database:**
- One central server stores all data.
- All branches or users must request data from this server.
- If the central database is hacked, *all data can be compromised.*

**Distributed Ledger:**
- Each branch (node) holds its own copy of the ledger.
- Any update made on one node automatically synchronizes across all others using a **peer-to-peer (P2P)** network.
- If one node is hacked or altered, discrepancies are easily detected by comparing it with other ledgers.

 **Analogy:**  
Think of it like a shared Google Sheet — when one person updates a cell, everyone sees it instantly. But unlike Google Sheets, blockchain uses cryptography to secure data so that no one can alter it without consensus.

### Discussion Questions

>  Is it required for all nodes to have access to all data?  
> Wouldn’t this demand enormous storage space for each node?

---

## Blocks

A **block** is a container of records, often representing transactions.  
Each block contains:
- **Data/Transactions**
- **A Timestamp**
- **A Cryptographic Hash of the Previous Block**

Once added to the chain, a block becomes **immutable** — meaning it cannot be modified without altering all subsequent blocks, which is computationally impractical.

 **In short:**
> A block = data + timestamp + cryptographic link to the previous block.

---

##  Cryptography

**Cryptography** is the study and practice of secure communication — protecting data from unauthorized access.

In blockchain, cryptography ensures:
- Data integrity
- Secure transaction verification
- Identity authentication

The **most widely used** cryptographic technique in blockchain is **SHA-256 (Secure Hash Algorithm 256-bit)**, used by Bitcoin and many others. It creates a unique, fixed-length hash output for any input, making tampering virtually impossible.

### Example of SHA-256 Hash

```text
Input:  Hello, Blockchain!
Output:  5d41402abc4b2a76b9719d911017c592
