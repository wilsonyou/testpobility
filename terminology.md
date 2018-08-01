# Terminology

This section gives details about the terms used in this document.

### Keypair

In the BUMO project, the keypair is the interface that generates the public key, private key, address, and signature . Only the ED25519 signature algorithm is supported during the signing process.

### Private Key

The private key is a string generated by the algorithm. The private key is a prerequisite for generating the public key and the address, and is also the basic element for completing the signature. The private key cannot be changed after it is generated. Once it is lost, it cannot be retrieved, so it needs to be kept safely.

### Public Key

The public key is a string generated based on the private key. It can verify the string encrypted by the private key. It does not expose the private key when transmitted between networks. It is also a necessary condition for generating an address.

### Address

The address is a string generated upon the public key. Similar to real-life addresses, contacts can't be found without an address, so transactions cannot be completed.

### Signature

The Signature refers to the process of encrypting and confirming transaction data by algorithm and private key and obtaining signature data. The user can verify the integrity and correctness of the transaction data through the signature data.

### Transaction

All operations that modify blockchain data in BUMO are called transactions, such as issuing assets, transferring assets, sending BUs, creating accounts, setting metadata and setting permissions, etc.

### Transaction Blob

The Transaction Blob is a hexadecimal string obtained by serializing a transaction object. Transaction serialization refers to the process of converting the state information of a transaction object into a string that can be stored and transmitted through the ProtoBuf data structure.

### Raw Private Key

The Raw Private Key is a byte array obtained by a random algorithm. The Raw Private Key is a prerequisite for generating a private key.

### Raw Public Key

The Raw Public Key is a byte array generated by processing the raw private key with the ED25519 algorithm. The Raw Public Key is a prerequisite for generating a public key.
