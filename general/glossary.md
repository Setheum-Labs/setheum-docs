# Glossary

The words / terms used in the Setheum Network that you would like to know.

The glossary used in this Wiki, Setheum White papers, in and around the Setheum Network.

[More] Need to add more Setheum Network related vocabulary in the future as more of the technology is being introduced and implemented.

## Setheum

The interoperable Ethereum compatible DeFi Blockchain Network for Stablecoins, smart contracts, Zero-Interest Loans, Trading, NFTs and all things DeFi built with Substrate framework.

## Authority

An authority is a generic term for the role in a blockchain that is able to participate in the consensus mechanisms. In GRANDPA, the authorities vote on chains they consider final. In BABE, the authorities are block producers. Authority sets can be chosen by mechanisms such as the NPoS algorithm.

### BABE

Blind Assignment of Block  Extension is Setheum's block production mechanism.

### Block

A collection of data, such as transactions, that together indicates a state transition of the blockchain

### Block explorer

An application that allows a user to explore the different blocks on a blockchain.

### BLS

Boneh-Lynn-Shacham (BLS) signatures have slow signing, very slow verification, require slow and much less secure pairing friendly curves, and tend towards dangerous malleability. Yet, BLS permits a diverse array of signature aggregation options far beyond any other known signature scheme, which makes BLS a preferred scheme for voting in consensus algorithms and for threshold signatures.

### Bonding

A process by which tokens can be "frozen" in exchange for some other benefit. For example, staking is a form of bonding for which you receive rewards in exchange for securing the network.

### Bridge

A parachain that acts as an intermediary between the Polkadot Relay Chain and an external chain, in such a way that it appears to the Relay Chain that the external chain is a parachain (i.e., meets the Polkadot Host's requirements of parachains). Bridges allow for interaction between other blockchains, such as Ethereum and Bitcoin, that are not natively compatible with Polkadot.

### Byzantine Fault Tolerance (BFT)

The property of a system that is tolerant of Byzantine faults; that is, a system where not only may individual subsystems fail, but it may not be clear if a particular subsystem has failed or not. That is, different observers on the system may not agree on whether or not the system has failed. Ensuring Byzantine fault tolerance is an important part of developing any distributed system.

### CDP

Collateralized Debt Position.


### Collator

A node that maintains a parachain by collecting parachain transactions and producing state transition proofs for the validators.

### Consensus

The process of a group of entities to agree on a particular data value (such as the ordering and makeup of blocks on a blockchain). There are a variety of algorithms used for determining consensus. The consensus algorithm used by both Setheum and Polkadot is GRANDPA.

### DApp

A generic term for a decentralized application, that is, one that runs as part of a distributed network as opposed to being run on a specific system or set of systems.

### DNAR

 The abbreviation and ticker for Setheum's " The Dinar" token. It serves as a [S.E.R.P.](https://wiki.setheum.xyz/general/glossary#) reserve asset to ensure SetCurrencies (Setheum Stablecoins) stay stable.

 ### Epoch

 An epoch is a time duration in the BABE protocol that is broken into smaller time slots. Each slot has at least one slot leader who has the right to propose a block. In Setheum, it is 4 hours (2,400 slots).

 ### Era

 A (whole) number of sessions, which is the period that the validator set (and each validator's active nominator set) is recalculated and where rewards are paid out.

### Extrinsic

State changes that come from the outside world, i.e. they are not part of the system itself. Extrinsics can take two forms, "[inherents](https://wiki.setheum.xyz/general/glossary#inherent)" and "[transactions](https://wiki.setheum.xyz/general/glossary#transaction)".

### Finality

The property of a block that cannot be reverted. Generally, created blocks are not final until some point in the future - perhaps never, in the case of "probabilistic finality". The Setheum Blockchain uses a deterministic finality gadget known as [GRANDPA](https://wiki.setheum.xyz/general/glossary#grandpa-finality-gadget).

### Finality Gadget

A mechanism that determines finality.

### FRAME

The collection of Substrate pallets (Substrate Runtime Modules).

### Genesis

The origin of a blockchain, also known as block 0. It can also be used to reference the initial state of the blockchain at origination.

### Governance

The process of determining what changes to the network are permissible, such as modifications to code or movement of funds. The governance system in Setheum is on-chain and revolves around Governance Council.

### Governance Council

An on-chain entity that consists of several on-chain accounts. The Council can act as a representative for "passive" (non-voting) stakeholders. Council members have two main tasks: proposing referenda for the overall stakeholder group to vote on and cancelling malicious referenda.

### GRANDPA Finality Gadget

GHOST-based Recursive ANcestor Deriving Prefix Agreement (GRANDPA). It is the finality gadget for Polkadot, Kusama, and Setheum, which allows asynchronous, accountable, and safe finality to the blockchain. For an overview of GRANDPA, see this Medium post: [https://medium.com/polkadot-network/polkadot-proof-of-concept-3-a-better-consensus-algorithm-e81c380a2372](https://medium.com/polkadot-network/polkadot-proof-of-concept-3-a-better-consensus-algorithm-e81c380a2372)

### Hard Fork

A permanent diversion of a blockchain that can occur quickly due to a high priority change in a consensus rule. Clients who follow a hard fork always need to upgrade their clients in order to continue following the upgraded chain. Hard forks are considered permanent divergences of a chain for which non-upgraded clients are following consensus rules incompatible to the ones followed by upgraded clients.

### Hard Spoon

Defined by Jae Kwon of Cosmos as "a new chain that takes into account state from an existing chain; not to compete, but to provide broad access." A non-contentious blockchain that inherits the state of the underlying blockchain and creates a new branch of the same blockchain.

### Inherent

Extrinsics that are "inherently true." Inherents are not gossiped on the network and are put into blocks by the block author. They are not provably true the way that the desire to send funds is, therefore they do not carry a signature. A blockchain's [runtime](https://wiki.setheum.xyz/general/glossary#runtime) must have rules for validating inherents. For example, timestamps are inherents. They are validated by being within some margin that each validator deems reasonable.

### LIBP2P

An open-source library for encrypted peer-to-peer communications and other networking functionality. More information at: https://libp2p.io/

### Liveness

The property of a distributed system that it will eventually come to some sort of consensus. A system stuck in an infinite loop would not be considered live, even if computations are taking place; a system that eventually provides a result, even if incorrect or it takes a long time, is considered to have liveness.

### NFT

Non-Fungible Token, meaning tokens that are one of a kind unique in their properties. Often called Cryptocollectibles.

### Node Explorer

A tool that gives you information about a node, such as the latest blocks sealed, finalized, and the current chain state as known by that node.

### Nominated Proof of Stake (NPoS)

A Proof-of-Stake system where nominators back validators with their own stake as a show of faith in the good behavior of the validator. Nominated Proof-of-Stake differs from the more generic concept Delegated Proof-of-Stake in that nominators are subject to loss of stake if they nominate a bad validator; delegators are not subject to loss of stake based on the behavior of the validator. Note that some other blockchain technologies may use the term Delegated Proof-of-Stake, even if delegators can be slashed. Both Polkadot and Setheum use the Phragmen method to allocate stake to nominees.

### Nominator

Accounts that select a set of validators to nominate by bonding their tokens. Nominators receive some of the validators' rewards, but are also liable for slashing if their nominated validators misbehave.

### On-chain Governance

A governance system of a blockchain that is controlled by mechanisms on the blockchain. On-chain governance allows decisions to be made in a transparent manner. Note that there are a variety of different algorithms for making these decisions, such as simple majority voting, adaptive quorum biasing, or identity-based quadratic voting.

### Oracle

Decentralised Oracles provide price feed information for assets on the Setheum network.

### Pallet (Module)

A Substrate runtime module. The pluggable building block for a Substrate chain.

### Parachain

A blockchain that meets several characteristics that allow it work within the confines of the Polkadot Host. Also known as "parallelized chain."

### Parachain Registry

A relatively simple database-like construct that holds both static and dynamic information on each chain.

### Polkadot

A heterogeneous, multi-chain network allowing various blockchains of different characteristics to perform arbitrary, cross-chain communication under shared security.

### Proof of Validity

A proof produced by parachain collators. Based on this proof and the parachain registry, a validator can verify that a parachain has properly executed its state transition function. Proofs of Validity go into the Relay Chain blocks.

### Proof of Work (PoW)

A method of selecting participants in a consensus system, typically the longest chain rule, in which participants try to solve a puzzle like finding a partial pre-image of a hash. Normally, a Proof-of-Work system can have any number of participants. PoW is used on the Bitcoin and Eth1.0 blockchains.

### Proposal

A potential function call to be voted on in a referendum. Proposals modify the behavior of the Setheum network, from minor parameter tuning all the way up to replacing the runtime code.

### Protocol

A system of rules that allows two or more entities of a communications system to transmit information. The protocol defines the rules, syntax, semantics and synchronization of communication and possible recovery methods.

### Random Seed

A random seed is pseudo-random number available on-chain. It is used in various places of the Setheum protocol, most prominently in [BABE](https://wiki.setheum.xyz/general/glossary#babe) the block production mechanism.

### Referendum

A vote on whether or not a proposal should be accepted by the network. Referenda may be initiated by the Governance Council or as the result of a previous proposal. Stakeholders vote on referenda, weighted by the size of their stake (i.e. number of SETM held).

### Runtime Module

A module that implements specific transition functions and features one might want to have in their runtime. Each module should have domain-specific logic. For example, a Balances module has logic to deal with accounts and balances. In Substrate, modules are called "pallets".

### SERP

Setheum Elastic Reserve Protocol is the main stablecoin stability system in Setheum. The SERP token alongside the [DNAR](https://wiki.setheum.xyz/general/glossary#dnar) is also one of the reserve assets of the Setheum Elastic Reserve Protocol.
### SETM

The Native token of the Setheum Network, used for staking and paying fees.

### SETR

The algorithmic stablecoin "Setter" is part of the Serp's stablecoin stability mechanism and is pegged to the value of 10 cents USD($0.1).

### SETUSD

The "SetDollar" is also an algorithmic stablecoin backed by [CDP](https://wiki.setheum.xyz/general/glossary#cdp) and the Setheum Elastic Reserve Protocol.

### SEVM

The SEVM is the Setheum-Ethereum Virtual Machine for deploying Ethereum standard smart contracts on Setheum just like on Ethereum's EVM with little to no changes to the smart contract's code.

### Safety

The property of a distributed system indicating that a particular state transition will not be reverted. GRANDPA provides deterministic safety. That is, for a state changed marked as "safe" or "final", one would require a hard fork to revert that change.

### Session

A session is a Substrate implementation term for a period of time that has a constant set of validators. Validators can only join or exit the validator set at a session change.

### Session Certificate

A message containing a signature on the concatenation of all the Session keys. Signed by the Controller.

### Session Key

Hot keys that are used for performing network operations by validators, for example signing GRANDPA commit messages.

### Slashing

The removal of a percentage of an account's SETM or as a punishment for a validator acting maliciously or incompetently (e.g., equivocating or remaining offline for an extended period of time).

### Soft Fork

A backwards compatible change to client code that causes upgraded clients to start mining a new chain. Requires a "vote-by-hashrate" of majority of miners in order to enact successfully. Soft forks are considered temporary divergences in a chain since non-upgraded clients do not follow the new consensus rules but upgraded clients are still compatible with old consensus rules.

### SPF

The Setheum Public Fund is a Non-Profit fund stewarded by the Setheum Foundation for altruism.

### Staking

The act of bonding SETM tokens by putting them up as "collateral" for a chance to produce a valid block (and thus obtain a block reward). Validators and nominators stake their SETM in order to secure the network.

### State transition function (STF)

A function that describes how the state of a blockchain can be transformed. For example, it may describe how tokens can be transferred from one account to another.

### Substrate

A modular framework for building blockchains. Polkadot, Kusama, Setheum, and other interesting projects are all built using Substrate. Chains built with Substrate will be easy to connect as parachains to the Polkadot Network and easier to communicate with eachother.

### Tabling

In both Setheum and Polkadot governance, bringing a proposal to a vote via referendum. Note that this is the British meaning of "tabling", which is different than the US version, which means "to postpone" a measure.

### Transaction

An extrinsic that is signed. Transactions are gossiped on the network and incur a transaction fee. Transactions are "provably true", unlike inherents. For example, one can prove that Alice wants to send funds to Bob by the fact that she signed a transfer-funds message with her private key.

### Validator

A node that secures the Blockhain by staking SETM, validating blocks and voting on consensus along with other validators.

### Voting

The process of stakeholders determining whether or not a referendum should pass. Votes are weighted by the number of SETM that the stakeholder account controls, votes in Setheum are performed in the Sequential Phragmen Method.

### Wallet

A program that allows one to store private keys and sign transactions for Setheum or other blockchain networks.

### WebAssembly / Wasm

An instruction format for a virtual, stack-based machine. Setheum Runtime Modules are compiled to WebAssembly, also known as Wasm.

### Witness

Cryptographic proof statements of data validity.
