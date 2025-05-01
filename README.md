## 🐦 Decentralized Twitter Clone (DApp)
Hi! I'm Isaac, a student at the University of East London, and this project is part of my final degree submission. It combines blockchain technology and modern web development to build a decentralized Twitter-like social media application.

This DApp leverages React for the frontend, Solidity for smart contracts, and Moralis for seamless Web3 integration. The goal was to demonstrate how social media platforms can be built with decentralized technologies, enabling user authentication through wallets, on-chain content posting, and NFT-based profiles.

## 🚀 Features
Login via MetaMask wallet.

Post tweets stored on the Polygon blockchain.

Use NFTs as profile pictures.

View and edit profiles.

Explore a public tweet feed powered by Moralis DB and Solidity smart contracts.

## 📁 Project Structure
pages/ – Home, Profile, and Settings views.

components/ – Sidebar, Rightbar, Tweet display.

src/tweets.sol – Smart contract for handling tweets.

src/tweetsABI.json – ABI used to connect frontend to smart contract.

## 🧪 Technologies Used
React

Solidity

Moralis

Web3UIKit

Polygon (Matic)

## 🛠 Installation Instructions

### 1. **Clone the Repository**
```bash
git clone https://github.com/izzie12/twitter-clone-dapp.git
cd twitter-clone-dapp
```

### 2. **Install Frontend Dependencies**
```bash
npm install
```

### 3. **Set Up a Moralis Server**

This project uses **Moralis** for Web3 authentication and database integration. You have to self host your own web3 moralis server to utilise this instruction.

#### 🔧 Option B: Self-Host Moralis (Advanced)
To self-host your own Moralis server using **Heroku**, **MongoDB**, and **Redis**:

1. Follow the official guide:  
   👉 [How to Set Up a Self-Hosted Web3 Server](https://developers.moralis.com/how-to-set-up-a-self-hosted-web3-server/)

2. Requirements:
   - MongoDB Atlas instance
   - Redis instance (e.g., from Redis Cloud or another provider)
   - GitHub account and Heroku CLI installed

3. After deploying:
   - Get the **Server URL** and **Application ID** from your deployment logs or environment settings.

---

### 4. **Create a `.env` File**
Add your credentials to a `.env` file in the project root:

```env
MORALIS_APP_ID=
MORALIS_SERVER_URL=
CONTRACT_ADDRESS=
```

---

### 5. **Start the React App**
```bash
npm start
```

---

### 6. **Deploy Smart Contract**
You can deploy the `tweets.sol` smart contract using [Remix IDE](https://remix.ethereum.org/) or **Hardhat** on the **Polygon Mumbai Testnet**.

After deployment:
- Save the contract address
- Update `tweetsABI.json` and relevant Web3 config in your frontend to point to the new contract.

---

Would you like me to also help you generate a `.env.example` file for users?
