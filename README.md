# Decentralized Image Sharing System

A decentralized application that allows users to upload and share images securely using Ethereum smart contracts and IPFS storage. The system removes the need for centralized servers and enables controlled access to images through blockchain-based permissions.

---

## Features

* **Decentralized Storage:** Images are uploaded and stored on IPFS using Pinata.
* **Smart Contract Integration:** Solidity smart contracts manage image ownership and access control.
* **Secure Access:** Users can grant or revoke access to their images for specific Ethereum addresses.
* **Blockchain Interaction:** MetaMask is used to interact with the Ethereum blockchain.
* **User-Friendly Interface:** A simple React-based interface for uploading and viewing images.

---

## Tech Stack

* **Solidity** – Smart contract development
* **Ethereum** – Blockchain platform
* **React.js** – Frontend user interface
* **Hardhat** – Smart contract development and deployment
* **IPFS / Pinata** – Decentralized file storage
* **MetaMask** – Ethereum wallet integration

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/skp4106/image-sharing-system.git
cd image-sharing-system
```

### 2. Install dependencies

Install Hardhat dependencies:

```bash
npm install
```

Install React frontend dependencies:

```bash
cd client
npm install
```

---

## Smart Contract Setup

Compile the smart contract:

```bash
npx hardhat compile
```

Deploy the contract:

```bash
npx hardhat run scripts/deploy.js --network <network-name>
```

After deployment, copy the **contract address** and update it inside the React application.

---

## Running the Application

Start the React application:

```bash
cd client
npm start
```

The application will run locally and connect to MetaMask for blockchain interaction.

---

## Configuration

* Create an account on **Pinata** to store images on IPFS.
* Obtain **Pinata API keys**.
* Update the API keys inside the `FileUpload.js` component.

---

## Usage

1. Connect MetaMask to the application.
2. Upload an image which will be stored on IPFS.
3. Grant access to specific Ethereum addresses if you want them to view the image.
4. Other users can view the images only if they have been granted permission through the smart contract.

---

## Future Improvements

* Image preview and gallery view
* Multi-user image management
* Improved UI/UX for better interaction
* Integration with additional decentralized storage solutions

---


