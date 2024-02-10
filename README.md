# Simple Blockchain Implementation using Singly Linked Lists

This project demonstrates a basic implementation of blockchain technology using singly linked lists in Java. Blockchain is a decentralized and distributed ledger technology that securely stores data through cryptographic hashing. Each block in the blockchain is represented as a node in the linked list, containing attributes such as timestamp, hash, previous hash, and data. The main concept behind blockchain is to ensure data security and integrity through the generation of unique hash values for each block.

## Working Principle

1. **Data Input:** The user inputs a string data that is to be stored in each node of the blockchain.
2. **Hashing:** The data undergoes hashing using a hashing method in Java. This generates a unique hash value for each input string.
3. **Block Connection:** Nodes are connected across the blockchain based on the generated hash values. The hash value of each block must match the previous hash value of the next block for the blockchain to remain valid.
4. **Blockchain Integrity:** The `isValid()` method checks the validity of the hash values in the blockchain. It indicates the block at which a breach has occurred if the hash values don't match.
5. **Data Display:** The `displayChain()` method displays the data stored in each block of the blockchain.
6. **Block Insertion:** The `insertBack()` method inserts new blocks of data at the back of the linked list, simulating the addition of new data to the blockchain.

## Hashing

Hashing is a fundamental technique used in blockchain to maintain the validity and integrity of data. It involves mapping a large chunk of data into small tables using a hashing function, also known as the message digest function. In this implementation, the `computeHash()` method in the node class generates a hash value for the stored data.

## Methods Overview

- `isValid()`: Checks the validity of hash values in the blockchain.
- `getScam()`: Allows the user to simulate a breach by changing a hash value.
- `displayChain()`: Displays the data stored in each block of the blockchain.
- `insertBack()`: Inserts new blocks of data at the back of the linked list.

## Blockchain Implementation Main

To run the blockchain implementation, execute the Main.java file. This file contains the main method to initiate the blockchain and perform operations such as inserting new blocks, checking blockchain validity, and simulating a breach.

## Sample Output

The code allows the user to change the hash value of any block in the blockchain, demonstrating how a breach affects the validity of the blockchain. Error messages are generated if there is a mismatch between hash values, indicating an invalid blockchain state.

This project serves as a simplified illustration of the basic concepts behind blockchain technology, showcasing its security features and the importance of hash values in maintaining data integrity.
