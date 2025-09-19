# Decentralized Voting App

A decentralized voting application built with **Vite**, **React**, **TypeScript**, and **Reown** packages for secure blockchain-based voting and proposal management.

## 🚀 Features

- **Decentralized Voting**: Transparent, immutable voting on the blockchain
- **Proposal Management**: Create, view, and manage voting proposals
- **Multi-Wallet Support**: Connect using various wallets via Reown integration
- **Real-time Results**: Live voting results and analytics
- **Admin Dashboard**: Administrative controls for proposal management
- **Responsive Design**: Mobile-friendly interface
- **Type Safety**: Full TypeScript implementation

## 🛠️ Tech Stack

### Frontend
- **Vite** - Fast build tool and development server
- **React 18** - UI library with hooks
- **TypeScript** - Type-safe JavaScript
- **Tailwind CSS** - Utility-first CSS framework

### Blockchain Integration
- **Reown** - Wallet connectivity and Web3 interactions
- **Wagmi** - React hooks for Ethereum
- **Viem** - TypeScript interface for Ethereum

### Smart Contracts
- **Solidity** - Smart contract language
- **Remix IDE** - Contract development and deployment

## 📋 Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- MetaMask or compatible Web3 wallet
- Access to Ethereum testnet (Sepolia recommended)

## 🔧 Installation

1. **Clone the repository**
   ```bash
      git clone <repository-url>
         cd decentralized-voting-app
            ```

            2. **Install dependencies**
               ```bash
                  npm install
                     ```

                     3. **Environment Setup**
                        ```bash
                           cp .env.example .env
                              ```
                                 
                                    Fill in your environment variables:
                                       ```env
                                          VITE_REOWN_PROJECT_ID=your_reown_project_id
                                             VITE_CONTRACT_ADDRESS=your_deployed_contract_address
                                                VITE_CHAIN_ID=11155111
                                                   ```

                                                   4. **Start development server**
                                                      ```bash
                                                         npm run dev
                                                            ```

                                                            ## 📁 Project Structure

                                                            ```
                                                            src/
                                                            ├── components/           # React components
                                                            │   ├── common/          # Reusable UI components
                                                            │   ├── voting/          # Voting-related components
                                                            │   ├── wallet/          # Wallet connection components
                                                            │   └── admin/           # Admin dashboard components
                                                            ├── pages/               # Page components
                                                            ├── hooks/               # Custom React hooks
                                                            ├── context/             # React context providers
                                                            ├── types/               # TypeScript type definitions
                                                            ├── utils/               # Utility functions
                                                            ├── lib/                 # Configuration files
                                                            └── styles/              # CSS styles

                                                            contracts/               # Smart contracts
                                                            ├── VotingContract.sol   # Main voting logic
                                                            ├── ProposalManager.sol  # Proposal management
                                                            ├── AccessControl.sol    # Access control mechanisms
                                                            └── interfaces/          # Contract interfaces
                                                            ```

                                                            ## 🔗 Smart Contract Deployment

                                                            1. **Open Remix IDE** at [remix.ethereum.org](https://remix.ethereum.org)

                                                            2. **Upload Contracts**
                                                               - Upload all `.sol` files from the `contracts/` directory

                                                               3. **Compile Contracts**
                                                                  - Select Solidity compiler version 0.8.19+
                                                                     - Compile all contracts

                                                                     4. **Deploy to Testnet**
                                                                        - Connect MetaMask to Sepolia testnet
                                                                           - Deploy `VotingContract.sol` first
                                                                              - Deploy `ProposalManager.sol` with VotingContract address
                                                                                 - Update `.env` with deployed contract addresses

                                                                                 ## 🎯 Usage

                                                                                 ### For Voters
                                                                                 1. **Connect Wallet** - Click "Connect Wallet" and select your preferred wallet
                                                                                 2. **Browse Proposals** - View active voting proposals
                                                                                 3. **Cast Votes** - Select your choice and submit transaction
                                                                                 4. **View Results** - Check real-time voting results

                                                                                 ### For Administrators
                                                                                 1. **Access Admin Panel** - Connect with admin wallet address
                                                                                 2. **Create Proposals** - Add new voting proposals
                                                                                 3. **Manage Voting** - Start/stop voting periods
                                                                                 4. **Monitor Activity** - View voting statistics and analytics

                                                                                 ## 🔧 Available Scripts

                                                                                 ```bash
                                                                                 # Development
                                                                                 npm run dev          # Start development server
                                                                                 npm run build        # Build for production
                                                                                 npm run preview      # Preview production build

                                                                                 # Code Quality
                                                                                 npm run lint         # Run ESLint
                                                                                 npm run type-check   # TypeScript type checking
                                                                                 ```

                                                                                 ## 🌐 Supported Networks

                                                                                 - **Ethereum Mainnet**
                                                                                 - **Sepolia Testnet** (recommended for testing)
                                                                                 - **Polygon**
                                                                                 - **Arbitrum**
                                                                                 - **Optimism**

                                                                                 ## 📊 Key Components

                                                                                 ### Wallet Integration
                                                                                 - Multi-wallet support via Reown
                                                                                 - Automatic network detection
                                                                                 - Transaction signing and confirmation

                                                                                 ### Voting System
                                                                                 - Secure proposal creation
                                                                                 - Time-bounded voting periods
                                                                                 - Immutable vote recording
                                                                                 - Real-time result calculation

                                                                                 ### Admin Features
                                                                                 - Proposal management
                                                                                 - Voting period controls
                                                                                 - User access management
                                                                                 - Analytics dashboard

                                                                                 ## 🔒 Security Features

                                                                                 - **Smart Contract Security**: Audited contract patterns
                                                                                 - **Access Control**: Role-based permissions
                                                                                 - **Vote Privacy**: Anonymous voting options
                                                                                 - **Timestamp Validation**: Secure voting periods
                                                                                 - **Replay Protection**: Prevent double voting

                                                                                 ## 🤝 Contributing

                                                                                 1. Fork the repository
                                                                                 2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
                                                                                 3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
                                                                                 4. Push to the branch (`git push origin feature/AmazingFeature`)
                                                                                 5. Open a Pull Request

                                                                                 ## 📄 License

                                                                                 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

                                                                                 ## 🆘 Support

                                                                                 For questions and support:
                                                                                 - Create an issue in the repository
                                                                                 - Check existing documentation
                                                                                 - Review smart contract comments

                                                                                 ## 🔗 Useful Links

                                                                                 - [Reown Documentation](https://docs.reown.com/)
                                                                                 - [Wagmi Documentation](https://wagmi.sh/)
                                                                                 - [Vite Documentation](https://vitejs.dev/)
                                                                                 - [Solidity Documentation](https://docs.soliditylang.org/)
                                                                                 - [Remix IDE](https://remix.ethereum.org/)

                                                                                 ---

                                                                                 **Built with ❤️ for decentralized governance**