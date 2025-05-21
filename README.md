# 🏡 Land Registry Using Blockchain

A decentralized application (DApp) designed to digitize and secure land registration, ownership, and asset transfer using the power of **Ethereum Blockchain**. This project leverages **Solidity** smart contracts to ensure immutability and transparency, eliminating fraud, corruption, and manipulation in traditional land records.

The frontend is built using **HTML/CSS** and interacts with the smart contract through **Web3.js** and **MetaMask** for secure, decentralized operations.

---

## 📌 Features

- 🔐 **User Registration** with identity verification fields
- 📄 **Land Asset Registration** with plot number, area, and valuation
- 📘 **Ownership Management** via Khatiyan (plot-wise ownership records)
- 🔎 **Data Retrieval** for users, assets, and khatiyan entries
- ❌ **User Removal** with optional payment feature
- 🖼️ Interactive UI styled with custom CSS for data viewing and entry

---

## 📖 Problem Statement

Land disputes and fraud are common due to centralized, paper-based land records. This system provides a **decentralized, transparent, and verifiable** method for land registration using blockchain — ensuring:
- Tamper-proof records
- Secure user and asset management
- Transparent historical ownership

---

## 🧱 Smart Contracts

### 📁 Structregistry.sol

This smart contract includes:
- `add_user()`: Registers a user with name, phone, and ID
- `get_user()`: Retrieves user details
- `add_asset()`: Adds land asset details
- `add_ownership()`: Maps ownership to plots
- `get_ownership()`: Retrieves ownership history
- `remove_user()`: Allows user removal with payable feature
- `get_array()`: Fetches all land assets

### 📁 Migrations.sol

Truffle-specific file for managing the contract deployment process.

---

## 🗂️ Project Structure

```bash
land-registry-blockchain/
├── contracts/
│   ├── Migrations.sol
│   └── Structregistry.sol
├── migrations/
│   ├── 1_initial_migration.js
│   └── 2_initial_migration.js
├── build/contracts/
│   ├── Migrations.json
│   └── Structregistry.json
├── css/
│   └── style.css
├── README.md
└── truffle-config.js

---

## ⚙️ Installation & Setup

### 1️⃣ Install Truffle

```bash
npm install -g truffle
truffle version
## 2️⃣ Install Ganache

```bash
npm install -g ganache-cli
ganache-cli

