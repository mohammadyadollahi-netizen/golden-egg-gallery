# Golden-Egg Metadata

## Metadata Architecture

Golden-Egg uses IPFS to store NFT metadata and artwork references.

The relationship between the NFT, blockchain, metadata, and artwork is:

```text
NFT
  ↓
ERC-721 Smart Contract
  ↓
tokenURI()
  ↓
IPFS Metadata
  ↓
Image CID
  ↓
Artwork
```

Each Golden-Egg token has its own metadata CID and artwork/image CID.

The blockchain stores the token URI reference, while the metadata and artwork are stored using IPFS.

---

---

## Token ID 0 — Legacy Record

Token ID `0` exists on the original Golden-Egg ERC-721 contract deployed on the Ethereum Sepolia Testnet.

### On-Chain Token URI

```text
ipfs://bafkreibs54kb2i76zh77fc3iyyikk773viuehc5owqkjih47k5qllmfxwi
```

### Original Mint Transaction

[View Token ID 0 Mint Transaction on Sepolia Etherscan](https://sepolia.etherscan.io/tx/0x2a9b252d9cb1a84200411654c19e083862e515e675cb9f59cb9b13041186111d)

### Metadata Recovery Status

The original metadata content could not be retrieved through the IPFS gateways and storage locations checked during this review.

The Token URI remains recorded on-chain. The original metadata JSON has not been recovered, and no replacement metadata has been created or presented as the original.

Token ID `0` is documented as a legacy record and is not included among the four featured artworks displayed in the Golden-Egg gallery.

The four featured artworks remain Token IDs `1`, `2`, `3`, and `4`.

This record documents the current investigation status. Failure to retrieve the metadata from the sources checked does not prove that no other copy exists.

---

# Golden-Egg #1

## Token ID

```text
1
```

## Token URI

```text
ipfs://bafkreickagoqhrpskvqyww4awlm66xmljibtpjeeawo3dzc6jdxz5yr2xa
```

## Metadata CID

```text
bafkreickagoqhrpskvqyww4awlm66xmljibtpjeeawo3dzc6jdxz5yr2xa
```

## Image CID

```text
bafybeibahee5qhjn5zh6x4xmx2lno26j3goqx2rschijikx4eig3sd5r6q
```

## Metadata

```json
{
  "name": "Golden-Egg",
  "description": "A digital artwork called Golden-Egg.",
  "image": "ipfs://bafybeibahee5qhjn5zh6x4xmx2lno26j3goqx2rschijikx4eig3sd5r6q"
}
```

### Naming Note

The original metadata name is:

```text
Golden-Egg
```

The gallery displays the artwork as:

```text
Golden-Egg #1
```

This is a display-label difference and does not change the Token ID or token URI.

---

# Golden-Egg #2

## Token ID

```text
2
```

## Token URI

```text
ipfs://bafkreihytiwjjsw4nr3dvgh5dyyzxw3qqs6jrbmomhxdioxrbhtblgw4t4
```

## Metadata CID

```text
bafkreihytiwjjsw4nr3dvgh5dyyzxw3qqs6jrbmomhxdioxrbhtblgw4t4
```

## Image CID

```text
bafybeihra6q5yvnyitntkpt3gd5eynkuzjhmsqfsvcbmuopvapmyqz6dku
```

## Metadata

```json
{
  "name": "Golden-Egg #2",
  "description": "A digital artwork from the Golden-Egg collection.",
  "image": "ipfs://bafybeihra6q5yvnyitntkpt3gd5eynkuzjhmsqfsvcbmuopvapmyqz6dku"
}
```

---

# Golden-Egg #3

## Token ID

```text
3
```

## Token URI

```text
ipfs://bafkreiev47cpkieizijczpb5ps7v3nbiave4f2onlzvoxbsdhd43uy4t3q
```

## Metadata CID

```text
bafkreiev47cpkieizijczpb5ps7v3nbiave4f2onlzvoxbsdhd43uy4t3q
```

## Image CID

```text
bafybeianohmded6d2qjqy3jrl72jlmrgvryjamme4kys6l6mnjhjpx75rq
```

## Metadata

```json
{
  "name": "Golden-Egg #3",
  "description": "A digital artwork from the Golden-Egg collection.",
  "image": "ipfs://bafybeianohmded6d2qjqy3jrl72jlmrgvryjamme4kys6l6mnjhjpx75rq",
  "attributes": [
    {
      "trait_type": "Collection",
      "value": "Golden-Egg"
    },
    {
      "trait_type": "Edition",
      "value": 3
    },
    {
      "trait_type": "Standard",
      "value": "ERC-721"
    }
  ]
}
```

---

# Golden-Egg #4

## Token ID

```text
4
```

## Token URI

```text
ipfs://bafkreidtosu2ey5ghnwzcbiu73ksedac52zw6j5ymqpriuxbk4xdbfy6xq
```

## Metadata CID

```text
bafkreidtosu2ey5ghnwzcbiu73ksedac52zw6j5ymqpriuxbk4xdbfy6xq
```

## Image CID

```text
bafybeiesrlomqtgsjyyfbms5wl3akirfih7kqbeqruqe5a77slqxwrx7vq
```

## Metadata Reference

The metadata for Token #4 is identified by the IPFS CID above.

The canonical token URI is:

```text
ipfs://bafkreidtosu2ey5ghnwzcbiu73ksedac52zw6j5ymqpriuxbk4xdbfy6xq
```

The artwork reference is:

```text
ipfs://bafybeiesrlomqtgsjyyfbms5wl3akirfih7kqbeqruqe5a77slqxwrx7vq
```

---

# Metadata Summary

| NFT           | Token ID | Metadata CID                                                  | Image CID                                                     |
| ------------- | -------: | ------------------------------------------------------------- | ------------------------------------------------------------- |
| Golden-Egg #1 |      `1` | `bafkreickagoqhrpskvqyww4awlm66xmljibtpjeeawo3dzc6jdxz5yr2xa` | `bafybeibahee5qhjn5zh6x4xmx2lno26j3goqx2rschijikx4eig3sd5r6q` |
| Golden-Egg #2 |      `2` | `bafkreihytiwjjsw4nr3dvgh5dyyzxw3qqs6jrbmomhxdioxrbhtblgw4t4` | `bafybeihra6q5yvnyitntkpt3gd5eynkuzjhmsqfsvcbmuopvapmyqz6dku` |
| Golden-Egg #3 |      `3` | `bafkreiev47cpkieizijczpb5ps7v3nbiave4f2onlzvoxbsdhd43uy4t3q` | `bafybeianohmded6d2qjqy3jrl72jlmrgvryjamme4kys6l6mnjhjpx75rq` |
| Golden-Egg #4 |      `4` | `bafkreidtosu2ey5ghnwzcbiu73ksedac52zw6j5ymqpriuxbk4xdbfy6xq` | `bafybeiesrlomqtgsjyyfbms5wl3akirfih7kqbeqruqe5a77slqxwrx7vq` |

---

# IPFS URI Format

Golden-Egg uses the standard IPFS URI format:

```text
ipfs://CID
```

For example:

```text
ipfs://bafkreihytiwjjsw4nr3dvgh5dyyzxw3qqs6jrbmomhxdioxrbhtblgw4t4
```

The `ipfs://` URI is the canonical decentralized reference.

Public HTTP gateways can be used to access IPFS content through a web browser, but gateway availability can vary.

---

# Metadata and Ownership

Metadata storage and NFT ownership are separate concepts.

The ERC-721 contract records token ownership and the token URI reference.

IPFS provides the referenced metadata and artwork content.

Therefore:

```text
Blockchain
= Ownership + Token Record + Token URI

IPFS
= Metadata + Artwork Reference
```

---

# Current Collection

The current Golden-Egg metadata structure contains four documented NFT records:

```text
Golden-Egg #1
Golden-Egg #2
Golden-Egg #3
Golden-Egg #4
```

Current collection progress:

```text
4 / 4
```

---

# Network

All current token records documented in this file belong to:

```text
Ethereum Sepolia Testnet
```

The current metadata records should not be interpreted as Ethereum Mainnet NFT records.

A future Mainnet deployment would use a separate contract and deployment record.
