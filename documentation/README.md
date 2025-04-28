# 📚 How the Fr42t3llo NFT Works

## 🔥 Functions Explained

- `safeTransferFrom(address _from, address _to, uint256 tokenId, bytes data)`  
  ➔ Safely transfers a token from `_from` to `_to` with additional `data`.  
  ➔ It **checks** if the recipient can receive NFTs.

- `safeTransferFrom(address _from, address _to, uint256 tokenId)`  
  ➔ Safely transfers a token without additional data.  
  ➔ Still **checks** if the recipient can handle NFTs.

- `transferFrom(address _from, address _to, uint256 tokenId)`  
  ➔ Transfers a token without checking if the recipient can receive NFTs.  
  ➔ ⚠️ **Warning**: If the recipient cannot handle NFTs, the NFT could be lost.

- `approve(address _approve, uint256 tokenId)`  
  ➔ Approves another address (`_approve`) to transfer the specified NFT (`tokenId`) on your behalf.

---

## 🧩 Main Features

### Minting
- Only the **contract owner** can mint new NFTs.
- Mint NFTs by calling the `safeMint(address to, uint256 tokenId, string calldata uri)` function.

### Token URI
- Each NFT links to metadata stored on **IPFS**.
- Metadata includes:
  - Name
  - Description
  - Image URL
  - Attributes

### Burning
- Any holder can **burn** (destroy) their NFT by calling the `burn(uint256 tokenId)` function.

---

## 📋 Metadata Example

```json
{
    "name": "myNFT",
    "description": "its my first nft, its very beautiful and have a 42 number",
    "image": "https://ipfs.io/ipfs/QmSxCqgaU84qxHR1Q77nyRatgZEfBQCG46y6sZnZcy4tHx",
    "attributes": [
        {
            "trait_type": "Artist",
            "value": "skasmi"
        }
    ]
}
