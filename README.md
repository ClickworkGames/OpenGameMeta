# GameMeta
**GameMeta is a Gaming Metadata Protocol**

GameMeta is a list of gaming networks and a game metadata catalogue. Users can use the information to connect their wallets and Web3 middleware providers to the appropriate game-related networks. Game studios & developers can use this info to build better web3 games and validate game-related contracts & details.

The goal is to build an open & social web3 games graph for the community to build trust and a secure way to validate games data.

GameMeta is a game-dev-curated, open protocol that any game developer uses and builds. It's part of the future of web3 game development.

## Game networks
A list of chains used in web3 games and can connect with user Web3 wallets. Superb Wallet Extension is the leading integrator, but many others may support multiple chains from here. Some entities here may be connected via Superb API or Superb Wallet API instead of Web3 wallet straight. This uses information that may also be seen on chainlist.org (https://github.com/ethereum-lists/chains).

The source data is in networks/chains. We do add CAIP-2 representation under chain data (features), but our naming is a bit simplified here “network-or-token-name+chainId-if-present” (https://github.com/ChainAgnostic/CAIPs/blob/master/CAIPs/caip-2.md). 

Remember that there are not only EVM-compatible chains, but we also want to unify and support other blockchains. Due to that, some records may be off the standard, and we do invite web3 & game developers to think about how to solve cross-chain and interoperability issues.

Module is Superb related parameter to define type of the network so we know which engine to use. Possible options are:

    - EVM (evm)
    - Solana (solana)
    - Cosmos (cosmos)
    - Bitcoin (bitcoin)
    - Polkadot (polkadot)
    - WAX (wax)
    - EOS (eos)
    - ICON (icon)
    - Obyte (obyte)

**Location: /networks
An example for Ethereum Mainnet is under “/networks/ethereum-1.json”.**

## Game metadata
Game metadata is vital so wallets and other web3 games and other projects can verify and interact with those contracts & tokens. Be aware of the metadata and other details needed to present it to other like it's meant to.

Game metadata has following core elements like name, description & logo. Network reference & smart contract information for all assets for each referenced network.

**Location: /games
An example for The Smurfs Society is under “/networks/the-smurfs-society.json”.**

## Adding your game data

Please find template from /template folder when adding your game metadata and network information.

When adding new game PR please also add game Terms of Conditions & Privacy Policy links and Whitepaper/Litepaper if exists. Also please add your game type - free to play, defi, play to earn etc...