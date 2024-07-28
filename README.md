# 🚀 Crowdfunding Platform - Arbitrum

A decentralized crowdfunding platform built with Next.js and Solidity smart contracts, deployed on Arbitrum for ultra-low gas fees and fast transactions.

## ✨ Features

- **🎯 Crowdfunding Campaigns**: Create and manage funding campaigns with custom goals
- **💰 Funding Tiers**: Multi-tier contribution system with different reward levels
- **🔒 Secure Smart Contracts**: Auditable contracts with automatic fund management
- **📱 Modern Interface**: Responsive UI built with Next.js 14 and Tailwind CSS
- **🌐 Web3 Native**: Full wallet integration using Thirdweb SDK v5
- **⚡ Arbitrum Powered**: Ultra-low transaction costs and fast confirmations

## 🏗️ Tech Stack

### Frontend
- **Next.js 14** - React framework with App Router
- **TypeScript** - Static type checking
- **Tailwind CSS** - Utility-first styling
- **Thirdweb SDK v5** - Web3 integration

### Smart Contracts
- **Solidity ^0.8.0** - Smart contract language
- **Foundry** - Development and testing framework
- **OpenZeppelin** - Security-focused libraries

### Blockchain
- **Arbitrum** - Layer 2 scaling solution
- **Low Gas Fees** - <$1 deployment costs
- **EVM Compatible** - Full Ethereum tooling support

## 🎮 Functionality

### For Campaign Creators
- Create campaigns with funding goals and deadlines
- Define custom funding tiers with different contribution amounts
- Manage campaign state (active/paused/completed)
- Withdraw funds when goals are achieved
- Track campaign performance and contributions

### For Contributors
- Browse active crowdfunding campaigns
- Contribute to different funding tiers
- Track personal contributions and history
- Automatic refunds for failed campaigns
- Real-time campaign progress updates

## 🚀 Getting Started

### Prerequisites
- Node.js 18+
- Yarn or npm
- Compatible wallet (MetaMask, WalletConnect, etc.)
- Some ETH on Arbitrum for transactions

### 1. Clone and Install

```bash
git clone <your-repo>
cd crowdfunding-arbitrum
yarn install
```

### 2. Environment Setup

Create a `.env.local` file:

```bash
NEXT_PUBLIC_TEMPLATE_CLIENT_ID=your_thirdweb_client_id
```

Get your Client ID from [Thirdweb Dashboard](https://thirdweb.com/dashboard)

### 3. Run Development Server

```bash
yarn dev
```

Visit [http://localhost:3000](http://localhost:3000)

### 4. Smart Contract Deployment (Optional)

To deploy your own contracts to Arbitrum:

```bash
cd crowdfundingcontracts
forge build
forge test
# Deploy to Arbitrum - update contract address in src/app/constants/contracts.ts
```

## 📁 Project Structure

```
├── src/
│   ├── app/                    # Next.js App Router
│   │   ├── campaign/[address]/ # Individual campaign page
│   │   ├── dashboard/[wallet]/ # User dashboard
│   │   ├── constants/          # Contract configurations
│   │   └── page.tsx           # Homepage
│   └── components/            # React components
│       ├── CampaignCard.tsx   # Campaign display card
│       ├── TierCard.tsx       # Funding tier card
│       ├── MyCampaignCard.tsx # Owner campaign card
│       └── Navbar.tsx         # Navigation component
├── crowdfundingcontracts/     # Smart contracts
│   ├── src/
│   │   ├── Crowdfunding.sol        # Main campaign contract
│   │   └── CrowdfundingFactory.sol # Factory deployment pattern
│   └── test/                  # Contract tests
└── public/                    # Static assets
```

## 🔧 Available Scripts

```bash
# Development
yarn dev

# Build
yarn build

# Production
yarn start

# Linting
yarn lint

# Smart Contracts
cd crowdfundingcontracts
forge build    # Compile contracts
forge test     # Run tests
forge deploy   # Deploy to network
```

## 🌐 Deployment

### Frontend Deployment
Deploy to Vercel, Netlify, or any hosting platform that supports Next.js:

```bash
yarn build
yarn start
```

### Smart Contract Deployment
1. Set up your wallet with Arbitrum ETH
2. Configure deployment script with your parameters
3. Deploy contracts to Arbitrum
4. Update contract address in `src/app/constants/contracts.ts`

## 💰 Gas Costs on Arbitrum

- **Contract Deployment**: <$1 USD
- **Campaign Creation**: ~$0.10
- **Contributing to Campaign**: ~$0.05
- **Withdrawing Funds**: ~$0.10

*Costs are approximately 90% lower than Ethereum mainnet*

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the project
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 🔗 Useful Links

- **Thirdweb Documentation**: [portal.thirdweb.com](https://portal.thirdweb.com)
- **Arbitrum Documentation**: [docs.arbitrum.io](https://docs.arbitrum.io)
- **Foundry Documentation**: [book.getfoundry.sh](https://book.getfoundry.sh)
- **Next.js Documentation**: [nextjs.org/docs](https://nextjs.org/docs)

---

**Built with ❤️ using Next.js, Solidity, and Arbitrum**