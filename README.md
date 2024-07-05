
# Decentralized Exchange

This is a decentralized exchange (DEX) built using React for the frontend, Solidity for the smart contracts, and Truffle for the development environment. The DEX allows users to trade ERC-20 tokens directly from their wallets without relying on a centralized authority.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technologies](#technologies)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Smart Contracts](#smart-contracts)
- [Frontend](#frontend)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project is a decentralized exchange that enables peer-to-peer trading of ERC-20 tokens. It leverages smart contracts to manage trades, ensuring trustless and transparent transactions.

## Features

- Trustless trading of ERC-20 tokens
- Wallet integration (e.g., MetaMask)
- Real-time updates of order book and trade history
- Responsive user interface

## Technologies

- React
- Solidity
- Truffle
- Web3.js
- MetaMask

## Requirements

Ensure you have the following installed:

- Node.js (v14 or later)
- npm or yarn
- Truffle (v5.4 or later)
- Ganache (for local blockchain development)

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/decentralized-exchange.git
cd decentralized-exchange
```

### 2. Install dependencies

```bash
# For backend (Truffle)
cd backend
npm install

# For frontend (React)
cd ../frontend
npm install
```

## Usage

### 1. Start Ganache

Start a local blockchain instance using Ganache.

### 2. Compile and migrate smart contracts

```bash
cd backend
truffle compile
truffle migrate --network development
```

### 3. Start the React frontend

```bash
cd ../DEX-main
npm start
```

### 4. Open the application

Open your browser and navigate to `http://localhost:3000`.

## Project Structure

```
decentralized-exchange/
├── backend/                 # Smart contracts and Truffle configuration
│   ├── contracts/           # Solidity contracts
│   ├── migrations/          # Migration scripts
│   ├── test/                # Test scripts
│   ├── truffle-config.js    # Truffle configuration file
│   └── build/               # Compiled contract artifacts
├── frontend/                # React frontend
│   ├── public/              # Public assets
│   ├── src/                 # Source files
│   │   ├── components/      # React components
│   │   ├── pages/           # React pages
│   │   ├── App.js           # Main app component
│   │   ├── index.js         # Entry point
│   └── package.json         # Frontend dependencies
└── README.md                # Project documentation
```

## Smart Contracts

The smart contracts are located in the `backend/contracts` directory. The main contract for the exchange is `Exchange.sol`, which manages orders, trades, and user balances.

### Contract Compilation and Migration

To compile and deploy the contracts to a local blockchain, use the following commands:

```bash
cd backend
truffle compile
truffle migrate --network development
```

## Frontend

The frontend is built with React and located in the `frontend` directory. It interacts with the smart contracts using Web3.js and MetaMask for wallet integration.

### Starting the Frontend

To start the React application, use:

```bash
cd frontend
npm start
```

This will run the app in development mode. Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.


