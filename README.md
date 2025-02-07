# Peer-to-Peer (P2P) Fund Transfer System Using Blockchain

## Project Overview
This project implements a secure and immutable Peer-to-Peer (P2P) fund transfer system using Blockchain technology. The blockchain structure ensures data security, transparency, and immutability through cryptographic validation. The system includes functionalities such as mining, block verification, transaction retrieval, and authorized block modifications for testing.

## By
**22IT113 - Smit Patel**

## Features Implemented
### 1. Blockchain Creation
- A blockchain is implemented with **5 blocks**, where the first block is the **Genesis Block**.
- Each block contains:
  - **Block Version**: Indicates the version of the block structure.
  - **Timestamp**: Exact time when the block was created.
  - **Transaction Data**: Fund transfer transactions between users.
  - **Previous Hash**: Ensures linkage to the previous block for integrity.

### 2. Mining Logic (Proof of Work)
- A cryptographic puzzle-based mining process is implemented.
- Miners must solve a mathematical puzzle (Proof of Work) to validate and add blocks.
- Ensures security and prevents unauthorized modifications.

### 3. Difficulty Level
- A **difficulty level** is set to control the time required for mining new blocks.
- Ensures proper validation and prevents rapid block creation.

### 4. Block Validation
- Verifies that each block:
  - Maintains a correct **previous hash linkage**.
  - Solves the cryptographic puzzle before being added to the blockchain.

### 5. Transaction History Retrieval
- Retrieves and displays all stored **financial transactions** from the blockchain.
- Ensures data transparency and accessibility.

### 6. Block Modification for Testing
- Allows **authorized modifications** of transaction data for auditing/debugging.
- Maintains an integrity check mechanism to prevent unauthorized changes.



