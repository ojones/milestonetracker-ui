# Milestone Tracker User Interface

The MilestoneTracker UI is a user interface for the [MilestoneTracker](https://github.com/Giveth/milestonetracker) contract and in future will be extended to cover the whole functionality of [Giveth DCO](https://github.com/Giveth/MVP) (Decantralised Charitable Organisation).

The application is written in React, interfaces directly with the Ethereum blockchain and the Giveth smart contracts. You can find the production version of this decentralized application (Dapp) and more information on the [Giveth website](https://giveth.io).

## How to run developer version
### Installing dependencies
1. Make sure you have installed [Node.js](https://nodejs.org/en/)
2. If not already, install Ethereum [testrpc](https://github.com/ethereumjs/testrpc)
    ```
    npm install -g ethereumjs-testrpc
    ```
3. Clone the repository
    ```
    # Clone the MilestoneTracker UI repository
    git clone git@github.com:Giveth/milestonetracker-ui.git

    cd milestonetracker-ui
    ```
4. Install dependencies
    ```
    npm install
    ```

### Running developer version
1. Run a local Ethereum node with JSON-RPC listening at port 8545 in deterministic mode.

  ```bash
  testrpc --deterministic
  ```

2. In new terminal window load the example data.

  ```bash
  cd node_modules/givethdirectory

  # Start Node.js
  node

  # Load the env.js script which automatically creates example data in the blockchain
  .load env.js
  ```

3. Start the dev server from the milestonetracker-ui directory.

  ```bash
  npm start
  ```

  Load [http://localhost:8080/](http://localhost:8080/) on your web browser.

### Production deployment
1. Run `npm run build` and upload `build/` to your server.
