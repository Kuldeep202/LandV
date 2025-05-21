# 🏡 Land Registry using Blockchain

This project is a decentralized **Land Registration System** developed using **Ethereum Smart Contracts** written in Solidity. It ensures tamper-proof registration of users, land assets, and ownership mappings using blockchain technology.

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

## 🧱 Smart Contracts

### 📁 `Structregistry.sol`
This is the core smart contract managing:

- `add_user()`: Adds a user with name, phone, and ID
- `get_user()`: Retrieves user details
- `add_asset()`: Adds land asset info
- `get_asset()`: Fetches asset details
- `add_khatiyan()`: Records ownership of land plots
- `get_khatiyan()`: Returns owners for a given plot
- `get_array()`: Retrieves all asset data
- `remove_user()`: Removes user with payable condition

### 📁 `Migrations.sol`
Default contract for managing Truffle migrations.

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
├── index.html
├── README.md
└── truffle-config.js
