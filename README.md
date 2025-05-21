# 🏡 LandChain – Blockchain-Based Land Registry Verification System

A decentralized **Land Registration and Verification System** built on the **Ethereum blockchain** to ensure secure, transparent, and tamper-proof land ownership records. It uses **Solidity smart contracts**, a **Web3.js-integrated frontend**, and **MetaMask** to facilitate trustless interactions between users and the system.

---

## 📌 Features

- 🔐 **User Registration** with identity verification (name, phone, ID)
- 🏞️ **Land Asset Registration** with plot number, area, and valuation
- 📘 **Ownership Mapping** for plot-wise ownership tracking
- 🔎 **Data Retrieval** for users, land assets, and ownership records
- ❌ **User Removal** (with optional payable functionality)
- 🖼️ **Interactive Frontend** styled with custom CSS

---

## 🧱 Smart Contracts

### `Structregistry.sol`

This contract includes:

```solidity
// Registers a new user
function add_user(string memory name, string memory phone, string memory id) public { ... }

// Retrieves user details by ID
function get_user(string memory id) public view returns (...) { ... }

// Adds a new land asset
function add_asset(string memory plot_no, string memory area, string memory value) public { ... }

// Fetches asset details by plot number
function get_asset(string memory plot_no) public view returns (...) { ... }

// Records ownership
function add_ownership(string memory plot_no, string memory owner_name) public { ... }

// Retrieves ownership
function get_ ownership(string memory plot_no) public view returns (...) { ... }

// Returns all land assets
function get_array() public view returns (...) { ... }

// Removes user (with payable condition)
function remove_user(string memory id) public payable { ... }
```
## 🗂️ Project Structure

```text
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
```
⚙️ Setup Instructions
🧰 Prerequisites
Node.js
Truffle – npm install -g truffle
Ganache
MetaMask browser extension
## 🛠️ Installation
Clone the repository and install dependencies:
```text
git clone https://github.com/yourusername/land-registry-blockchain.git
cd land-registry-blockchain
npm install
truffle compile
truffle migrate --network development
```
## ▶️ Running the App
Open Ganache and ensure Truffle is using the correct RPC and network ID.
Compile and deploy the contracts:
```text
truffle compile
truffle migrate --reset
```
Open index.html in your browser.
Connect MetaMask to your local Ganache blockchain.
Start interacting with the system via the UI.

## 💻 Technologies Used
Solidity – Smart contract programming
Truffle – Development framework for Ethereum
Ganache – Local Ethereum blockchain
Web3.js – JavaScript interface for Ethereum
MetaMask – Wallet and Ethereum provider
HTML/CSS – Frontend structure and styling

## 🛡️ Security Notes
Only use on testnets before considering mainnet deployment.
Avoid storing sensitive or personal data on-chain.
Validate user input both in the frontend and smart contract.


