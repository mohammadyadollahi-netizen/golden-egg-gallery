````markdown
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

```
