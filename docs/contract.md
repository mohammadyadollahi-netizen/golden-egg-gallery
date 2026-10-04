# Golden-Egg Smart Contract

## Overview

The Golden-Egg collection uses an ERC-721 smart contract deployed on the Ethereum Sepolia Testnet.

The contract manages NFT token ownership and stores the metadata URI associated with each token.

---

## Contract Information

| Property          | Value                                        |
| ----------------- | -------------------------------------------- |
| Collection        | `Golden-Egg`                                 |
| Symbol            | `GEGG`                                       |
| Standard          | `ERC-721`                                    |
| Network           | Ethereum Sepolia Testnet                     |
| Contract Address  | `0x389C1Dc0Df1eE889ac9EefCE84787E83F9069167` |
| Contract Owner    | `0x71C508b0B799D5941B91DA7966029C53c1d6F692` |
| Compiler          | `v0.8.30+commit.73712a01`                    |
| Optimization      | No                                           |
| Optimization Runs | 200                                          |
| EVM Version       | Prague                                       |
| License           | MIT                                          |
| Verification      | Verified on Sepolia Etherscan                |

---

## Explorer

https://sepolia.etherscan.io/address/0x389C1Dc0Df1eE889ac9EefCE84787E83F9069167

---

# ERC-721 Functions

The contract supports standard ERC-721 functionality including:

### `balanceOf(address owner)`

Returns the number of NFTs owned by an address.

### `ownerOf(uint256 tokenId)`

Returns the current owner of a specific NFT.

### `getApproved(uint256 tokenId)`

Returns the approved address for a specific token.

### `isApprovedForAll(address owner, address operator)`

Returns whether an operator is approved to manage all NFTs belonging to an owner.

### `name()`

Returns:

```text
Golden-Egg
```

### `symbol()`

Returns:

```text
GEGG
```

### `supportsInterface(bytes4 interfaceId)`

Checks whether the contract supports a particular interface such as ERC-721.

### `tokenURI(uint256 tokenId)`

Returns the metadata URI associated with a specific NFT.

---

# Mint Function

The contract contains an owner-restricted mint function:

```solidity
mint(string memory uri)
```

The mint process:

1. Creates the next token ID.
2. Mints the NFT to the contract owner.
3. Stores the supplied metadata URI.
4. Returns the newly created token ID.

The current collection contains four minted tokens.

---

# Token URI Records

## Golden-Egg #1

```text
tokenURI(1)

ipfs://bafkreickagoqhrpskvqyww4awlm66xmljibtpjeeawo3dzc6jdxz5yr2xa
```

## Golden-Egg #2

```text
tokenURI(2)

ipfs://bafkreihytiwjjsw4nr3dvgh5dyyzxw3qqs6jrbmomhxdioxrbhtblgw4t4
```

## Golden-Egg #3

```text
tokenURI(3)

ipfs://bafkreiev47cpkieizijczpb5ps7v3nbiave4f2onlzvoxbsdhd43uy4t3q
```

## Golden-Egg #4

```text
tokenURI(4)

ipfs://bafkreidtosu2ey5ghnwzcbiu73ksedac52zw6j5ymqpriuxbk4xdbfy6xq
```

---

# Ownership Records

The four documented tokens are associated with the project owner address:

```text
0x71C508b0B799D5941B91DA7966029C53c1d6F692
```

## Token #1

```text
ownerOf(1)

0x71C508b0B799D5941B91DA7966029C53c1d6F692
```

## Token #2

```text
ownerOf(2)

0x71C508b0B799D5941B91DA7966029C53c1d6F692
```

## Token #3

```text
ownerOf(3)

0x71C508b0B799D5941B91DA7966029C53c1d6F692
```

## Token #4

```text
ownerOf(4)

0x71C508b0B799D5941B91DA7966029C53c1d6F692
```

---

# Metadata Capability

The contract stores the token URI during the mint process.

The current contract interface does not provide a general-purpose public metadata-update function such as:

```text
setTokenURI()
```

Therefore, the existing token URI references should be treated as part of the current deployed contract configuration.

For a future production deployment, metadata-management requirements should be considered during smart-contract design before deployment.

---

# Current Token Records

| Token         | Token ID | Status |
| ------------- | -------: | ------ |
| Golden-Egg #1 |      `1` | Minted |
| Golden-Egg #2 |      `2` | Minted |
| Golden-Egg #3 |      `3` | Minted |
| Golden-Egg #4 |      `4` | Minted |

Current progress:

```text
4 / 4 Minted
```

---

# Testnet Status

The contract is deployed on:

```text
Ethereum Sepolia Testnet
```

The current deployment is used for:

* NFT development
* ERC-721 learning
* blockchain verification
* IPFS metadata testing
* collection development
* public project presentation

This contract should not be represented as an Ethereum Mainnet deployment.

A future Ethereum Mainnet deployment would be a separate production deployment with a different contract address and deployment record.

---

# Contract Address

```text
0x389C1Dc0Df1eE889ac9EefCE84787E83F9069167
```

**Network:** Ethereum Sepolia Testnet

**Collection:** Golden-Egg

**Symbol:** GEGG

**Standard:** ERC-721

**Status:** Verified
