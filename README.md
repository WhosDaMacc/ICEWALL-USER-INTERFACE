
Ice Wall

Welcome to Ice Wall – an augmented reality-powered financial metaverse, where users can interact with each other, play games, train virtual pets called Navitars, and earn rewards within the app. The app is built with blockchain integration for secure, transparent financial transactions and smart contract management.

Table of Contents
	•	Overview
	•	Features
	•	Technology Stack
	•	Installation
	•	Frontend Structure
	•	Backend Structure
	•	Smart Contracts
	•	Contributing
	•	License

Overview

Ice Wall is an immersive financial metaverse designed to provide users with a unique experience combining blockchain technology, augmented reality (AR), and real-time location-based features. Players engage in activities such as:
	•	Navitar Combat: Players battle with their virtual pets, Navitars, using skills, strategies, and special abilities.
	•	Team-based Training: Players can form teams to work together and unlock unique perks.
	•	Blockchain Integration: All transactions, rewards, and progression are tracked on the blockchain for transparency.
	•	Augmented Reality: Players explore the world around them, interact with businesses, and earn rewards in real time.

Features
	•	Navitars: Customizable virtual pets that can be trained, upgraded, and battle each other in the Ice Wall metaverse.
	•	AR Integration: Use augmented reality to interact with virtual elements and track real-world locations for in-game rewards.
	•	DAO Voting: Decentralized governance allowing users to vote on platform decisions and manage team progression.
	•	Item Inventory: Users can collect and manage items that boost performance, train Navitars, or gain special abilities.
	•	User Profile & Team Info: Each player has a profile with stats, a team, and a unique identity within the Ice Wall metaverse.
	•	Location-based Rewards: Players can earn rewards by checking in to businesses and hubs in both rural and urban areas.

Technology Stack
	•	Frontend:
	•	React for UI components and routing.
	•	Redux for global state management.
	•	Web3.js and MetaMask for blockchain interaction.
	•	Three.js or AR.js for augmented reality features.
	•	Backend:
	•	Node.js and Express for API and server-side logic.
	•	PostgreSQL with PostGIS for geolocation-based data.
	•	Redis for real-time session management.
	•	Blockchain:
	•	Ethereum (Polygon) for smart contracts and cryptocurrency integration.
	•	Solidity for developing the smart contracts.
	•	IPFS for storing media files.

Installation

Prerequisites
	•	Node.js >= 16.x.x
	•	npm or yarn
	•	MetaMask installed for interacting with the blockchain

1. Clone the repository

git clone https://github.com/your-username/ice-wall.git
cd ice-wall

2. Install dependencies

npm install

3. Run the frontend and backend

For local development, start both the frontend and backend in separate terminals.

Frontend:

cd /ice-wall-ui
npm start

Backend:

cd /ice-wall-backend
npm start

4. Access the app

Once the servers are running, access the app at:
	•	Frontend: http://localhost:3000
	•	Backend: http://localhost:5000

Frontend Structure

/ice-wall-ui
│
├── /src
│   ├── /components
│   │   ├── /User
│   │   ├── /Team
│   │   ├── /Shared
│   │   └── App.jsx
│   ├── /hooks
│   ├── /services
│   ├── /context
│   ├── /styles
│   └── index.js
├── /public
└── package.json

Key Components
	•	User Profile: Displays the user’s profile, inventory, and Navitar stats.
	•	Team: Lists the members and stats for teams, along with perks and team progression.
	•	Shared Components: Includes global UI elements such as headers, footers, and loading spinners.

Backend Structure

/ice-wall-backend
│
├── /src
│   ├── /controllers
│   ├── /models
│   ├── /routes
│   ├── /services
│   └── /utils
├── /migrations
├── /config
└── server.js

Key Endpoints
	•	GET /user/:id: Fetches user profile data.
	•	POST /user/:id/items: Adds new items to a user’s inventory.
	•	GET /team/:id: Fetches team data, including members and stats.
	•	GET /navitar/:id/fight: Initiates a Navitar battle.

Smart Contracts

Overview

The Ice Wall smart contract suite is responsible for managing the blockchain aspects of the platform, including user staking, rewards, and decentralized governance.

Key Contracts:
	•	GlacierToken (GLC): The native utility token for the Ice Wall ecosystem.
	•	StakingContract: Manages staking rewards for users.
	•	GovernanceContract: Handles user voting and decision-making.

How to Deploy Smart Contracts
	1.	Install dependencies:

npm install --save-dev truffle web3


	2.	Configure your truffle-config.js to include the appropriate network and wallet settings.
	3.	Deploy to Polygon:

truffle migrate --network polygon

Contributing

We welcome contributions to the Ice Wall project! To contribute:
	1.	Fork the repository.
	2.	Create a new branch for your feature or bug fix.
	3.	Make your changes and test thoroughly.
	4.	Submit a pull request with a description of your changes.

License

This project is licensed under the MIT License – see the LICENSE file for details.

Feel free to customize and expand the sections as your project evolves.