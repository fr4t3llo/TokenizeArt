# 🚀 Deployment Guide

## ⚙️ Deployment Tools
- [Remix IDE](https://remix.ethereum.org/)
- MetaMask extension
- Filebase for uploading metadata to IPFS

---

## 🛤 Deployment Steps

### 1. Upload Image to IPFS
- Use Filebase to upload your NFT image.
- Copy the IPFS CID link.

### 2. Create Metadata JSON
- Create a JSON file that includes the image link, description, and other attributes.
- Upload this JSON file to Filebase.
- Get the CID of the metadata JSON.

### 3. Prepare Contract in Remix
- Open Remix IDE.
- Create a new Solidity file.
- Paste your `Fr42t3llo.sol` contract code.
- Compile it using Solidity version `0.8.20`.

### 4. Deploy Contract
- Connect MetaMask to the Holesky network.
- Deploy the contract by passing your MetaMask address as `initialOwner`.

### 5. Mint NFT
- After deployment, use the `safeMint` function:
  - `to`: Wallet address to receive the NFT.
  - `tokenId`: Unique ID (e.g., 1, 2, 3...).
  - `uri`: IPFS link to the metadata (starting with `ipfs://` or `https://ipfs.io/ipfs/...`).

### 6. Verify Deployment
- Check on Etherscan for the Holesky network (if available).
- View the minted NFT using tools like OpenSea testnets (if supported) or NFT viewer platforms.

---
