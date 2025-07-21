# 🔗 NFT DApp

A full-stack decentralized application (DApp) that allows users to mint, manage, and view NFTs. Built with React, Hardhat, Solidity, and integrated with Metamask, Alchemy, and IPFS via Pinata.

---

## 🚀 Tech Stack & Dependencies

Ensure you have the following installed:

- **Node.js & NPM** – https://nodejs.org
- **Hardhat** – https://hardhat.org/hardhat-runner/docs/getting-started
- **Metamask** – https://metamask.io/download/
- **Ganache (Optional)** – https://trufflesuite.com/ganache/

Optional tools (for enhanced Web3 experience):

- **Alchemy** – https://auth.alchemyapi.io/signup
- **Pinata (for IPFS storage)** – https://www.pinata.cloud/

---

## 🛠️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/adams-id/hardhat-nft-dapp.git
cd nft-dapp
```

### 2. Install Dependencies

```bash
npm install
```

---

## ⚙️ Environment Configuration

Create a `.env` file in the root directory and add the following:

### For React apps:

```
VITE_ALCHEMY_API_URL=https://eth-sepolia.g.alchemy.com/v2/YOUR_API_KEY
VITE_ALCHEMY_API_KEY=YOUR_API_KEY
VITE_PRIVATE_KEY=YOUR_METAMASK_PRIVATE_KEY
VITE_PRIVATE_KEY2=OPTIONAL_SECOND_PRIVATE_KEY

VITE_CONTRACT_ADDRESS=YOUR_DEPLOYED_CONTRACT_ADDRESS
VITE_CONTRACT_ADDRESS_LOCAL=YOUR_LOCAL_CONTRACT_ADDRESS

VITE_PINATA_KEY=YOUR_PINATA_API_KEY
VITE_PINATA_SECRET=YOUR_PINATA_SECRET
```

### For scripts:

```
ALCHEMY_API_URL=https://eth-sepolia.g.alchemy.com/v2/YOUR_API_KEY
ALCHEMY_API_KEY=YOUR_API_KEY
PRIVATE_KEY=YOUR_METAMASK_PRIVATE_KEY
PRIVATE_KEY2=OPTIONAL_SECOND_PRIVATE_KEY

CONTRACT_ADDRESS=YOUR_DEPLOYED_CONTRACT_ADDRESS
CONTRACT_ADDRESS_LOCAL=YOUR_LOCAL_CONTRACT_ADDRESS

PINATA_KEY=YOUR_PINATA_API_KEY
PINATA_SECRET=YOUR_PINATA_SECRET
```

---

## 🔧 Running the Project

### 1. Start Local Blockchain (Optional)

Using Hardhat:

```bash
npx hardhat node
```

Or use Ganache manually.

---

### 2. Deploy the Smart Contract

To a local blockchain:

```bash
npx hardhat run scripts/deploy.js
```

To Sepolia (or another testnet):

```bash
npx hardhat run scripts/deploy.js --network sepolia
```

---

### 3. Start the React App

```bash
npm start
```

Open in your browser at: [http://localhost:3000](http://localhost:3000)

---

### 4. Run the NFT Mint Script

```bash
npx hardhat run scripts/mint-nft.js
```

---

## 📦 Project Structure

```
├── contracts/           # Solidity smart contracts
├── scripts/             # Deployment and interaction scripts
├── src/                 # React frontend code
├── .env                 # Environment variables
├── hardhat.config.js    # Hardhat configuration
└── package.json
```

---

## 🧪 Networks

Supports deployment to:

- Local Hardhat network
- Sepolia testnet (via Alchemy)

---

## 🖼 IPFS Integration

- Media files for NFTs are pinned using **Pinata**.
- Token metadata is uploaded to **IPFS** and referenced in the smart contract.

---

## 📃 License

MIT – feel free to use, modify, and share this project.
