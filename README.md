

---

```markdown
# HTML Fund Me (Foundry + Frontend)

A simple **Fund Me DApp** built with [Foundry](https://book.getfoundry.sh/) (Solidity smart contracts) and a frontend in **HTML/JavaScript**.  
This project allows users to connect their wallet (like MetaMask) and fund the contract, while the contract owner can withdraw funds.

---

## 🚀 Features
- Connect your wallet via MetaMask
- Fund the smart contract with ETH
- Track balances and contributions
- Withdraw functionality restricted to the owner
- Local testing with [Anvil](https://book.getfoundry.sh/anvil/)

---

## 📂 Project Structure
```

html-fund-me-cu/
├── src/            # Solidity contracts (FundMe.sol)
├── script/         # Deployment scripts
├── test/           # Foundry unit and integration tests
├── frontend/       # HTML + JavaScript frontend
├── broadcast/      # Deployment logs (ignored in .gitignore)
└── README.md       # Project documentation

````

---

## 🛠 Prerequisites
- [Foundry](https://book.getfoundry.sh/getting-started/installation) (Solidity toolkit)
- [Node.js](https://nodejs.org/) (for frontend dependencies, if any)
- [MetaMask](https://metamask.io/) (for interacting with the contract)

---

## ⚡ Usage

### 1. Compile contracts
```bash
forge build
````

### 2. Run tests

```bash
forge test -vvv
```

### 3. Start a local blockchain

```bash
anvil
```

### 4. Deploy the contract

In another terminal:

```bash
forge script script/DeployFundMe.s.sol --rpc-url http://127.0.0.1:8545 --private-key <your-private-key> --broadcast
```

### 5. Open the frontend

* Open `index.html` in your browser
* Connect MetaMask (set to the correct network)
* Fund or withdraw from the contract 🎉

---

## 🌍 Deployment

* Local: via Anvil
* Testnet: you can deploy to Sepolia, Holesky, or any Ethereum testnet (update RPC URL & private key)

---

## 📜 License

This project is licensed under the MIT License.
Feel free to use, modify, and share!

