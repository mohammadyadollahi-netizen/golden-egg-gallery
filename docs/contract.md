````markdown
# Golden-Egg Smart Contract

## Overview

The Golden-Egg collection uses an ERC-721 smart contract deployed on the Ethereum Sepolia Testnet.

The contract manages the NFT tokens in the collection and exposes public read functions for collection information, token ownership, approvals, and token metadata references.

---

## Contract Information

| Property | Value |
|---|---|
| Collection | `Golden-Egg` |
| Symbol | `GEGG` |
| Standard | `ERC-721` |
| Network | Ethereum Sepolia Testnet |
| Contract Address | `0x389C1Dc0Df1eE889ac9EefCE84787E83F9069167` |
| Owner | `0x71C508b0B799D5941B91DA7966029C53c1d6F692` |
| Verification | Verified on Sepolia Etherscan |

### Explorer

https://sepolia.etherscan.io/address/0x389C1Dc0Df1eE889ac9EefCE84787E83F9069167

---

## Public Read Functions

The verified contract currently exposes the following public read functions through Etherscan:

### `balanceOf(address owner)`

Returns the number of NFTs owned by an address.

### `getApproved(uint256 tokenId)`

Returns the approved address for a specific token.

### `isApprovedForAll(address owner, address operator)`

Returns whether an operator is approved to manage all NFTs belonging to an owner.

### `name()`

Returns the collection name.

Expected value:

```text
Golden-Egg
````

### `owner()`

Returns the contract owner.

Current value:

```text
0x71C508b0B799D5941B91DA7966029C53c1d6F692
```

### `ownerOf(uint256 tokenId)`

Returns the current owner of a specific NFT.

### `supportsInterface(bytes4 interfaceId)`

Used to check whether the contract supports a specific interface such as ERC-721.

### `symbol()`

Returns the collection symbol.

Expected value:

```text
GEGG
```

### `tokenURI(uint256 tokenId)`

Returns the metadata URI associated with a specific NFT.

---

## Token URI Verification

### Token #1

```text
tokenURI(1)

ipfs://bafkreickagoqhrpskvqyww4awlm66xmljibtpjeeawo3dzc6jdxz5yr2xa
```

### Token #2

```text
tokenURI(2)

ipfs://bafkreihytiwjjsw4nr3dvgh5dyyzxw3qqs6jrbmomhxdioxrbhtblgw4t4
```

---

## Ownership Verification

### Token #1

```text
ownerOf(1)

0x71C508b0B799D5941B91DA7966029C53c1d6F692
```

### Token #2

```text
ownerOf(2)

0x71C508b0B799D5941B91DA7966029C53c1d6F692
```

---

## Contract Capability Note

The current public read interface does not expose a function such as:

```text
setTokenURI()
```

Therefore, the existing token URI references should be treated as part of the current contract configuration.

For future production deployments, metadata-update requirements should be considered during smart-contract design before deployment.

---

## Testnet Status

This contract is deployed on:

```text
Ethereum Sepolia Testnet
```

It is currently being used for development, verification, and collection-building purposes.

A future Ethereum Mainnet deployment would be a separate production deployment.

````

### 2) `docs/collection.md`

```markdown
# Golden-Egg Collection

## Collection Overview

Golden-Egg is a digital art NFT collection built using ERC-721, Ethereum Sepolia, and IPFS.

The initial collection is planned as three artworks.

| Artwork | Token ID | Status |
|---|---:|---|
| Golden-Egg #1 | `1` | ✅ Minted |
| Golden-Egg #2 | `2` | ✅ Minted |
| Golden-Egg #3 | `3` | 🔜 Planned |

### Current Progress

```text
2 / 3
````

---

## Golden-Egg #1

### Identification

* Token ID: `1`
* Display name: `Golden-Egg #1`
* Standard: ERC-721
* Network: Ethereum Sepolia

### Owner

```text
0x71C508b0B799D5941B91DA7966029C53c1d6F692
```

### Metadata

```text
ipfs://bafkreickagoqhrpskvqyww4awlm66xmljibtpjeeawo3dzc6jdxz5yr2xa
```

### Image

```text
ipfs://bafybeibahee5qhjn5zh6x4xmx2lno26j3goqx2rschijikx4eig3sd5r6q
```

### Note

The original on-chain metadata name is:

```text
Golden-Egg
```

The Gallery uses the display label:

```text
Golden-Egg #1
```

This naming difference is documented here and does not change the current token ID or token URI.

---

## Golden-Egg #2

### Identification

* Token ID: `2`
* Name: `Golden-Egg #2`
* Standard: ERC-721
* Network: Ethereum Sepolia

### Owner

```text
0x71C508b0B799D5941B91DA7966029C53c1d6F692
```

### Metadata

```text
ipfs://bafkreihytiwjjsw4nr3dvgh5dyyzxw3qqs6jrbmomhxdioxrbhtblgw4t4
```

### Image

```text
ipfs://bafybeihra6q5yvnyitntkpt3gd5eynkuzjhmsqfsvcbmuopvapmyqz6dku
```

### Mint Transaction

```text
0xcf29b6aee1de1efb2e6e28710c0f97c2d1781ad2543483ee047499c109c33794
```

Transaction:

https://sepolia.etherscan.io/tx/0xcf29b6aee1de1efb2e6e28710c0f97c2d1781ad2543483ee047499c109c33794

---

## Golden-Egg #3

Golden-Egg #3 is planned for a future release.

The artwork, IPFS image, metadata, and Token ID 3 will be added only after the artwork and metadata are finalized.

---

## Collection Contract

```text
0x389C1Dc0Df1eE889ac9EefCE84787E83F9069167
```

Network:

```text
Ethereum Sepolia Testnet
```

Symbol:

```text
GEGG
```

---

## Official Gallery

https://mohammadyadollahi-netizen.github.io/golden-egg-gallery/

---

## Repository

https://github.com/mohammadyadollahi-netizen/golden-egg-gallery

````

### 3) `docs/metadata.md`

```markdown
# Golden-Egg Metadata

## Metadata Architecture

Golden-Egg uses IPFS to store NFT metadata and artwork references.

The relationship is:

```text
NFT
  ↓
ERC-721 Contract
  ↓
tokenURI()
  ↓
IPFS Metadata
  ↓
Image CID
  ↓
Artwork
````

---

## Golden-Egg #1

### Token URI

```text
ipfs://bafkreickagoqhrpskvqyww4awlm66xmljibtpjeeawo3dzc6jdxz5yr2xa
```

### Metadata CID

```text
bafkreickagoqhrpskvqyww4awlm66xmljibtpjeeawo3dzc6jdxz5yr2xa
```

### Image CID

```text
bafybeibahee5qhjn5zh6x4xmx2lno26j3goqx2rschijikx4eig3sd5r6q
```

### Metadata

```json
{
  "name": "Golden-Egg",
  "description": "A digital artwork called Golden-Egg.",
  "image": "ipfs://bafybeibahee5qhjn5zh6x4xmx2lno26j3goqx2rschijikx4eig3sd5r6q"
}
```

---

## Golden-Egg #2

### Token URI

```text
ipfs://bafkreihytiwjjsw4nr3dvgh5dyyzxw3qqs6jrbmomhxdioxrbhtblgw4t4
```

### Metadata CID

```text
bafkreihytiwjjsw4nr3dvgh5dyyzxw3qqs6jrbmomhxdioxrbhtblgw4t4
```

### Image CID

```text
bafybeihra6q5yvnyitntkpt3gd5eynkuzjhmsqfsvcbmuopvapmyqz6dku
```

### Metadata

```json
{
  "name": "Golden-Egg #2",
  "description": "A digital artwork from the Golden-Egg collection.",
  "image": "ipfs://bafybeihra6q5yvnyitntkpt3gd5eynkuzjhmsqfsvcbmuopvapmyqz6dku"
}
```

---

## Golden-Egg #3 Metadata Standard

For the future #3 artwork, the intended metadata structure is:

```json
{
  "name": "Golden-Egg #3",
  "description": "A digital artwork from the Golden-Egg collection.",
  "image": "ipfs://IMAGE_CID"
}
```

The final `IMAGE_CID` will be inserted only after the #3 artwork is uploaded to IPFS.

---

## IPFS Gateway Examples

Metadata can be viewed through:

```text
https://dweb.link/ipfs/METADATA_CID
```

Artwork can be viewed through:

```text
https://dweb.link/ipfs/IMAGE_CID
```

The canonical NFT references remain the `ipfs://` URIs stored in the metadata and returned by `tokenURI()`.

````
