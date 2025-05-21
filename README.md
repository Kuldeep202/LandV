# 🏡 LandV – Blockchain-based Land Registry Verification System
LandV is a decentralized application (dApp) that uses blockchain technology to securely manage land ownership records. Built on Ethereum using Solidity smart contracts, it eliminates the risks of forgery, corruption, and manual error in traditional land registry systems by offering a tamper-proof, transparent, and automated solution.

# 🔍 Key Highlights:
✅ Tamper-Proof Records: All user and land asset data is stored on the blockchain, ensuring it cannot be altered or deleted once registered.

👤 User Identity Verification: Users must register with details like name, ID, and phone number to ensure authentic entries.

📄 Land Asset Registration: Users can register land plots with details such as plot number, area, and valuation.

📘 Ownership Mapping: Track ownership of land plots using khatiyan-style records for better traceability.

🔄 Ownership Transfer and Management: Smart contracts manage the assignment or reassignment of land ownership.

🔎 Decentralized Data Retrieval: Easily fetch user data, asset details, and ownership records from the blockchain.

🧾 Smart Contract Enforcement: All operations are enforced by code on the Ethereum network—no third-party approvals needed.

🌐 MetaMask Integration: Secure user transactions via MetaMask wallet support.

🖥️ Interactive Frontend: Built using HTML/CSS and Web3.js to allow real-time interaction with the blockchain backend.


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


