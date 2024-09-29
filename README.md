
# 📝 Anonymous Review Platform (Blockchain-Based)

**Anonymous Review** is a decentralized platform where users can submit and access anonymous reviews with the security and transparency of blockchain technology. Reviews are stored immutably, ensuring that feedback remains untampered, trustworthy, and completely anonymous.

🔗 **Live Project:** [Anonymous Review on GitHub](https://github.com/Vikas8346/Anonymous-Review)

📽️ **Demo Video:** [Watch the Demo](./sample-video.mp4)

## 📖 Table of Contents
- [🌟 Features](#-features)
- [🛠️ Tech Stack](#️-tech-stack)
- [🚀 Getting Started](#-getting-started)
- [💻 Smart Contract](#-smart-contract)
- [📘 Usage](#-usage)
- [🤝 Contributing](#-contributing)
- [📜 License](#-license)

## 🌟 Features
- 🔒 **Complete Anonymity:** Submit reviews without revealing your identity.
- ⛓️ **Blockchain-Backed Integrity:** Reviews are stored on a public blockchain, making them tamper-proof.
- 🌐 **Transparent Access:** Anyone can access the reviews and verify their authenticity.
- 🧾 **Smart Contract Verification:** All interactions are handled via a smart contract, ensuring secure and transparent operations.

## 🛠️ Tech Stack
- **Frontend:**
  - React ⚛️
  - HTML/CSS/JavaScript 🎨
- **Backend:**
  - Solidity 📝 (Smart Contracts)
  - Web3.js 🌐 (Blockchain Interaction)
  - IPFS 📦 (Decentralized Storage)
- **Blockchain:**
  - Ethereum (or any EVM-compatible chain) ⛓️
- **Development Environment:**
  - Truffle/Hardhat 🛠️
  - MetaMask 🦊 (Wallet Integration)

## 🚀 Getting Started

### Prerequisites
Ensure you have the following installed:

- Node.js (v14 or later) 🌳
- NPM (Node Package Manager) 📦
- Truffle/Hardhat (for smart contract development) ⚙️
- MetaMask (for managing blockchain transactions) 🦊

### Installation Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Vikas8346/Anonymous-Review.git
   cd Anonymous-Review
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Compile the smart contract:**
   ```bash
   truffle compile
   ```

4. **Deploy the smart contract (using Ganache or a testnet):**
   ```bash
   truffle migrate
   ```

5. **Start the frontend server:**
   ```bash
   npm start
   ```

6. **Configure MetaMask:**
   - Connect to your local blockchain (Ganache) or the network where the contract is deployed.
   - Import the account used for contract deployment into MetaMask.

## 💻 Smart Contract

The smart contract in this project is responsible for securely handling reviews. It stores the reviews immutably, ensuring that once a review is submitted, it cannot be altered or removed.

### Contract Features:
- **Submit Review:** Anonymously submit a review which is stored on the blockchain.
- **Retrieve Reviews:** Access all reviews stored on the blockchain.
- **Anonymity:** The contract ensures that users' identities remain anonymous by not storing personal data.

### Solidity Contract Example:
```solidity
// Function to submit a review
function submitReview(string memory _review) public {
    reviews.push(Review({content: _review, reviewer: msg.sender}));
    reviewCount++;
    emit ReviewSubmitted(msg.sender, reviewCount);
}

// Function to retrieve reviews
function getReviews() public view returns (Review[] memory) {
    return reviews;
}
```

## 📘 Usage

1. **Submit a Review:**
   - Navigate to the "Submit Review" page.
   - Enter your feedback in the form.
   - Confirm the transaction in MetaMask to anonymously submit the review to the blockchain.

2. **View Reviews:**
   - Go to the "View Reviews" section.
   - All reviews stored on the blockchain will be displayed transparently.

3. **MetaMask Interaction:**
   - Ensure your MetaMask wallet is connected and set to the correct network.
   - Each submission will require a blockchain transaction, so make sure you have enough test Ether for gas fees.

## 🤝 Contributing

Contributions are welcome! 🎉

If you'd like to contribute to this project, please follow these steps:

1. **Fork** the repository 🍴
2. **Create a branch** for your feature (`git checkout -b feature-branch`) 🌿
3. **Make your changes** and commit them (`git commit -m 'Add cool feature'`) ✍️
4. **Push to the branch** (`git push origin feature-branch`) 🚀
5. **Open a pull request** on GitHub 👨‍💻

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

🚀 **Anonymous Review Platform** is a game-changer for secure, transparent, and anonymous feedback. Be a part of the decentralized future and try it out today!

