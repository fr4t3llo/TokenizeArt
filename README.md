# 🖼️ Project Name: Fr42t3llo NFT

## 📜 Short Description
This repository contains the smart contract for **Fr42t3llo**, an ERC-721 Non-Fungible Token (NFT).  
The NFT is deployed on the Ethereum Holesky test network, with assets (image + metadata) stored on IPFS (InterPlanetary File System) via Filebase.  
It allows the contract owner to mint NFTs with custom metadata.

---

## 🛠 Platforms and Tools Used
- **Remix IDE**:  
  Chosen for its simplicity and browser-based environment, Remix is ideal for fast prototyping and deploying smart contracts without the need for local blockchain setups.

- **MetaMask**:  
  Used for managing accounts and signing transactions securely.

- **Filebase + IPFS**:  
  Chosen to host the NFT metadata and images permanently in a decentralized way.

- **Ethereum Holesky Network**:  
  Selected because it is a test network specifically designed for large-scale testing of Ethereum applications.

---

## 🔤 Language
- The smart contract is written in **Solidity (version ^0.8.20)**.

---

## 🔎 Repository Structure

| Path             | Description                                          |
|------------------|------------------------------------------------------|
| `/contracts/`    | Contains the `Fr42t3llo.sol` smart contract.          |
| `/deployment/`   | Scripts and instructions on how to deploy the contract. |
| `/documentation/`| Details on how the project works, including minting instructions. |

---

## ✅ Features
- Mint new NFTs with custom URIs (only by the owner).
- NFTs are burnable (can be destroyed by their holders).
- Each NFT points to its unique metadata hosted on IPFS.
- Ownership management is handled through OpenZeppelin's `Ownable` extension.

---
