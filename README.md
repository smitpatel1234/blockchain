<<<<<<< HEAD
# Blockchain Demo
A web-based demonstration of blockchain concepts.

[![Blockchain 101 - Demo](https://img.youtube.com/vi/_160oMzblY8/0.jpg)](https://www.youtube.com/watch?v=_160oMzblY8)

This is a very basic visual introduction to the concepts behind a blockchain. We introduce 
the idea of an immutable ledger using an interactive web demo that is available here:

http://andersbrownworth.com/blockchain/

## Setup
Get the code:

```
git clone https://github.com/anders94/blockchain-demo.git
```

Install dependencies:

```
cd blockchain-demo
npm install
```
Run the server:

```
npm start
```

OR

```
./bin/www
```
#For windows: if the above command didn't work, use this (make sure you have Node.js installed in your system):
```
node ./bin/www      
```

Point a web browser at the demo:

```
http://localhost:3000
```

## Setup using Docker

Get the code:

```
git clone https://github.com/anders94/blockchain-demo.git
```

Run the Docker setup:

```
cd blockchain-demo
docker-compose up -d
```

Point a web browser at the demo:

```
http://localhost:3000
```

## Optional Configuration
You can adjust the "number of zeros" required by the demo by editing the first two lines of
`public/javascripts/blockchain.js`.

Because there are 16 possible characters in a hex value, each time you increment the difficulty
by one you make the puzzle 16 times harder. In my testing, a difficulty of 6 requires a
maximumNonce well over 500,000,000.

If you adjust the difficulty above 4, blocks will show up as not mined because the demo data
assumes 4 zeros for a signed block. For example, on the `http://localhost:3000/block` page
with a difficulty of 6, the first nonce that works is `8719932` yielding a hash of
`000000669445c22167511857d8f3b822b331c3342f25dfdcb326e35c1a7aa267`. This gets out of hand fairly
quickly though. Here's some time estimates at the various thresholds.

|digits|nonce|time estimate|
|------|-------|-------------|
|4|500,000|15 minutes
|5|8,000,000|4 hours
|6|128,000,000|3 days
|7|2,048,000,000|a month
|8|32,768,000,000|2 years
|9|524,288,000,000|30 years
|10|8,388,608,000,000|481 years
|11|134,217,728,000,000|7,690 years
|12|2,147,483,648,000,000|123,036 years
|13|34,359,738,368,000,000|1,968,581 years
|14|549,755,813,888,000,000|31,497,291 years
|15|8,796,093,022,208,000,000|503,956,662 years

In the production bitcoin blockchain, block `458,091` has the hash digest
`00000000000000000000011246f099d94f91628d71c9d75ad2f9a06e2beb7e92`. That's 21 zeros in a row!
That one block would take this software approximately 8,454,989,768,407,765 years to mine.

### Public Private Key Demo

The 2nd part of the 101 session:
* https://github.com/anders94/public-private-key-demo

## Send Thanks

![](public/images/qr.png)

Bitcoin gratefully accepted: `1K3NvcuZzVTueHW1qhkG2Cm3viRkh2EXJp`
=======
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



>>>>>>> 9b592b233dfcc631446200482d6e8ea22fe19601
