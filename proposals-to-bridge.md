# Bridging To & From Ethereum mainnet

This document outlines solutions and discussions about bridging. Mostly focusing on bridging Ethereum mainnet to side-chains, or Ethereum mainnet to other major chains.

> I spent 2 yrs analyzing Bitcoin's code until I felt confident to hold btc. I Found 8 vulns along the way. 
> A bridge contract is the most adversarial scenario: open code, no upgrade, unlocking tokens for people that usually don't know the risks. 
> Even a blockchain is easier to fix
> 
> [Sergio Demian Lerner, May 18, 2020](https://twitter.com/SDLerner/status/1262436758828003329)


## Writings and Discussions

[Trustless Two-Way Bridges With Side Chains By Halting](https://ethresear.ch/t/trustless-two-way-bridges-with-side-chains-by-halting/5728) - very good overview of techniques (and interesting proposal) by @adlerjohn, @matt, @mikerah, and @villanuevawill

[Common Interoperability Approaches](https://github.com/renproject/ren/wiki/Interoperability) - Ren documentation which also covers the common approaches of Atomic Swaps, Native Interoperability, Synthetics, and Multi-sigs

[Two-way bridges between eth1 and eth2](https://ethresear.ch/t/two-way-bridges-between-eth1-and-eth2/6286)

[Plasma Bridge – connecting two Layer-1 chains with a plasma chain](https://ethresear.ch/t/plasma-bridge-connecting-two-layer-1-chains-with-a-plasma-chain/2890) - EthResearch discussion

### Atomic Swaps

[A Complete Beginner's Guide To Atomic Swaps](https://www.forbes.com/sites/lukefitzpatrick/2019/09/02/a-complete-beginners-guide-to-atomic-swaps/#90a7c4617846) - Forbes article

[Atomic Cross-Chain Swaps](https://arxiv.org/pdf/1801.09515.pdf) - July 2018 paper by Maurice Herlihy

[Atomic Crosschain Transactions for Ethereum Private Sidechains](https://arxiv.org/pdf/1904.12079.pdf) - paper from ConsenSys / PegaSys, School of Information Technology and Electrical Engineering, University of Queensland, Australia

[Is it possible to make atomic swap between Ethereum and POS chain?](https://ethresear.ch/t/is-it-possible-to-make-atomic-swap-between-ethereum-and-pos-chain/5051/2) - EthResearch discussion

[Succinct Atomic Swap](https://gist.github.com/RubenSomsen/8853a66a64825716f51b409be528355f) and [diagram](https://gist.github.com/RubenSomsen/8853a66a64825716f51b409be528355f#file-succinctatomicswap-svg) - a proposal by Ruben Somsen

## Interop between Ethereum mainnet and side-chains

### Connext Spacefold

"Spacefold demonstrates how Connext can be used to build an internet-of-l2-chains/shards. Users can instantly and seamlessly transfer value between chains/shards, and eventually even make atomic cross-chain contract calls. Most importantly, this can happen in a way where users dont need to know what chain/rollup/shard they are on to begin with."

- [GitHub repo](https://github.com/connext/spacefold)
- [Demo / website](https://www.spacefold.io/)

### Matic Swaps

Note: this solution is based on the ["More Viable Plasma"](https://ethresear.ch/t/more-viable-plasma/2160) protocol. All Plasma protocol implementations are bridged to an Ethereum blockchain, but have a lengthily challenge period. 

"The construction includes introduction of a new method in each associated asset contract - ERC721 and ERC20 on matic plasma chain, called transferWithSig."
- [GitHub repo](https://github.com/nglglhtr/asset-swap-tutorial)
- [Documentation](https://docs.matic.network/docs/develop/advanced/swap-assets)
- [Description of mapping of assets from Eth1 to Matic Network](https://docs.matic.network/docs/develop/advanced/mapping-assets)

### POA TokenBridge

- [Documentation](https://docs.tokenbridge.net/)
- [GitHub repo](https://github.com/poanetwork/tokenbridge)
- [Introducing the ERC20 to ERC20 TokenBridge](https://medium.com/poa-network/introducing-the-erc20-to-erc20-tokenbridge-ce266cc1a2d0) (also supports "Arbitrary-Message" / arbitrary contract method invocation)
- [Related Forum Discussions](https://forum.poa.network/c/tokenbridge/25)
- older/deprecated [POABridge GitHub repo](https://github.com/poanetwork/poa-bridge)

### Baseline Protocol

"The Baseline Protocol is an open source initiative that combines advances in cryptography, messaging, and blockchain to execute secure and private business processes at low cost via the public Ethereum Mainnet. The protocol will enable confidential and complex collaboration between enterprises without leaving any sensitive data on-chain."
- [GitHub repo](https://github.com/ethereum-oasis/baseline)
- [Documentation](https://docs.baseline-protocol.org/)

### OpenST Mosaic
- [GitHub repo](https://github.com/OpenST/mosaic-contracts)
- [White Paper](https://github.com/OpenST/mosaic-contracts/blob/develop/docs/mosaicv0.pdf)

### Grid+ Relay Networks

- [Efficiently Bridging EVM Blockchains](https://blog.gridplus.io/efficiently-bridging-evm-blockchains-8421504e9ced) - discusses designs used in Relay Networks V2

### AltCoin atomic swapping

DEX in which "developers can lock ether tokens in an Ethereum smart contract that specifies the funds will only be sent if an equal amount of bitcoin is sent to a bitcoin address during a specific time window".

- [Altcoin](https://altcoin.io/)
- ["ethatomicswap" GitHub repo](https://github.com/AltCoinExchange/ethatomicswap)
- [Update about atomic swals and plasma](https://blog.altcoin.io/august-update-mobile-ux-atomic-swaps-and-plasma-dex-v2-94680ff9db30) - 9/18/2018 


## Interop between major blockchains

### tBTC - bridge to Bitcoin

"tBTC is a sidechain designed to allow BTC holders a way to earn yield with their Bitcoin trustlessly, using decentralized finance (DeFi) applications. TBTC is an ERC-20 token that is minted when a user provides proof of their BTC deposit. A TDT is a non-fungible ERC-721 token (NFT) that represents a claim to a deposit’s underlying UTXO on the Bitcoin blockchain. Because TBTC is interchangeable with TDT, they can be considered two states of the same fundamental asset."

- [Website](https://tbtc.network/)
- [Overview](https://tbtc.network/news/2020-05-06-3-in-1-how-tbtc-is-erc-20-erc-721-and-stablecoin/)
- [Specification](https://docs.keep.network/tbtc/index.pdf)

### REN - bridge to Bitcoin

"Open protocol that provides access to inter-blockchain liquidity for all decentralized applications. RenVM uses secret computation/storage to implement general purpose interoperability between new and existing blockchains. It defines special 'secret contracts' that can be used to send digital assets, and generic data, from one blockchain to another."

- [Website](https://renproject.io/)
- [GitHub repo](https://github.com/renproject/ren)
- [RenVM Overview](https://medium.com/renproject/how-renvm-actually-works-c2f76a2630c4)
- [RenVM Documentation](https://github.com/renproject/ren/wiki/Introduction)

### ChainSafe ChainBridge - bridge to Cosmos

- [Announcement](https://medium.com/chainsafe-systems/chainsafe-building-chainbridge-49d51ff2e0a2)
- [GitHub repo](https://github.com/ChainSafe/ChainBridge)
- Ethermint network [website](https://ethermint.zone/) / [GitHub repo](https://github.com/ChainSafe/ethermint)

### Snowfork - bridge to Polkadot

- [Overview](https://snowfork.substack.com/p/a-trustless-general-purpose-polkadot)
- [Website](http://www.snowfork.com/)

### dogethereum

- [Using Superblocks to Bridge Dogecoin to Ethereum](https://github.com/dogethereum/docs/blob/master/superblocks/superblocks-white-paper.pdf)
- [dogethereum documentation](https://github.com/dogethereum/docs)

### Wanchain atomic swapping

- [Website](https://www.wanchain.org/)
- Wanchain cross-chain contracts [GitHub Repo](https://github.com/wanchain/wanchain-crosschain-contracts)
- [CoinDesk Article](https://www.coindesk.com/wanchains-bridge-to-the-ethereum-blockchain-is-now-open/)

### Decred atomic swapping

(No swapping for ETH?)

"These tools do not operate solely on-chain. A side-channel is required between each party performing the swap in order to exchange additional data. This side-channel could be as simple as a text chat and copying data."

- On-chain atomic swaps [GitHub Repo](https://github.com/decred/atomicswap)
- [Overview Blog Post](https://blog.decred.org/2017/09/20/On-Chain-Atomic-Swaps/)


## Major blockchains which are oriented toward interop

### Eth2

The Execution Environments, operating within shards, will be able to transact seamlessly. The Eth1 staking mechanism for Eth2 validators is actually a bridge! There are also proposals to bridge between Eth2 and Eth1 (which will continue to function within / as a shard).

[Cross-shard DeFi composability](https://ethresear.ch/t/cross-shard-defi-composability/6268) - classic post/discussion on the issue by Vitalik Buterin

[How can we facilitate cross-shard communication?](https://github.com/ethereum/wiki/wiki/Sharding-FAQ#how-can-we-facilitate-cross-shard-communication) - Sharding PAQ

**Two-way Bridges Between Eth1 and Eth2**
- [EthResearch discussions about the Eth1-Eth2 Transition](https://ethresear.ch/c/eth1-to-eth2-transition/38)
- [Two-way bridges between eth1 and eth2](https://ethresear.ch/t/two-way-bridges-between-eth1-and-eth2/6286) - proposal and EthResearch discussion

### Polkadot

A fully decentralized "federation" of chains, allowing both open and closed networks to have trust-free access to each other, for exchanging value and for processing data. A "relay chain" coordinates consensus and transaction delivery between member chains. Blockchains are bridged to the Polkadot Nework. This is accomplished with "parachains", which are parallelizable, highly specialized blockchains implemented for each Polkadot participant. Parachains attach to the security provided by the relay chain rather than providing their own.

- [An Introduction to Polkadot](https://blog.stephantual.com/web-three-revisited-part-two-introduction-to-polkadot-what-it-is-what-it-aint-657782051d34)
- [Website](https://polkadot.network/)
- [Polkadot Paper](https://github.com/polkadot-io/polkadotpaper/raw/master/PolkaDotPaper.pdf)(PDF)
- [Overview of "parachain"](https://medium.com/polkadot-network/polkadot-the-parachain-3808040a769a)
- [Now Live: Polkadot POC](https://medium.com/@polkadotnetwork/now-live-polkadot-proof-of-concept-1-3e718512a8d)

### Cosmos Hub

The Cosmos hub connects to zones via IBC (inter-blockchain communication) protocol) and keeps a record of the total number of tokens in each zone. Because all inter-zone transfers go through the Cosmos Hub, you can send tokens from one zone to another without the need for a liquid exchange or trusted third party between zones.

- [Website](https://cosmos.network/intro/hub)
- [Ethermint](https://ethermint.zone/)
- [Introducing the Ethereum Peg Zone](https://blog.cosmos.network/the-internet-of-blockchains-how-cosmos-does-interoperability-starting-with-the-ethereum-peg-zone-8744d4d2bc3f)
- [The Shanghai Accord - Ethereum Scaling Agreement](https://blog.cosmos.network/the-shanghai-accord-ethereum-scaling-agreement-via-cosmos-at-wanxiang-global-blockchain-summit-354efa27b158)

### AION

"This Aion bridging mechanism is an entire Byzantine Fault Tolerant protocol where the majority of nodes a.k.a “Bridge Validators” must agree on transactions or state changes on one network, then pass that transaction to another network to trigger smart contracts."

- [Website](https://aion.network/)
- [reddit discussion](https://www.reddit.com/r/AionNetwork/comments/8gkam6/what_makes_aions_token_swap_with_ethereum_so/dycztsj/)
- [Alpha release Blog Post](https://blog.aion.network/aion-token-bridge-alpha-version-2d3655d9d861)

## What's Happening?

Recently not enough information, GitHub updates, etc. to determine status

### Loom Interop
- [Announcement of Ethereum, EOS, TRON interop solution](https://medium.com/loom-network/connecting-ethereum-eos-and-tron-making-blockchain-interoperability-a-reality-e5ef6c67716)

## Defunct Projects

While these are defunct, they contain very useful insights!

### BTC Relay

Ethereum contract for Bitcoin SPV. The main functionality it provides are: verification of a Bitcoin transaction,  optionally relay the Bitcoin transaction to any Ethereum contract storage of Bitcoin block headers, inspection of the latest Bitcoin block header stored in the contract.

- ["btcrelay" GitHub Repo](https://github.com/ethereum/btcrelay)
- [etherscan.io page for 0x41f274c0023f83391de4e0733c609df5a124c3d4](https://etherscan.io/address/0x41f274c0023f83391de4e0733c609df5a124c3d4)

### Canto

By applying a similar logic as that found within traditional networking protocols such as TCP/IP, we propose a novel approach toward the optimization of the existing Ethereum network in a manner that only requires a marginal degree of additional development to the existing system.

- [Overview](https://medium.com/whiteblock/canto-overview-5f8f3a6f7dad) by Trenton Van Epps
- [Specification](https://github.com/canto-ethereum/spec/blob/master/canto.md)
- [FAQ](https://github.com/canto-ethereum/spec/blob/master/canto.md#faq)

### Giveth "ghetto bridge"

- [Update mentioning bridge](https://medium.com/giveth/where-are-we-now-status-of-the-giveth-dapp-5f5ba7791d12)




