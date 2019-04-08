# Bridging To & From Ethereum

This document outlines solutions and discussions about bridging.

---

## POA Network Bridge

- [Introducing POA Bridge and POA-20](https://medium.com/poa-network/introducing-poa-bridge-and-poa20-55d8b78058ac)
- [GitHub repo](https://github.com/poanetwork/poa-bridge)
- [Specification](https://hackmd.io/s/rkLKGbJLX#)

## Polkadot

A fully decentralized "federation" of chains, allowing both open and closed networks to have trust-free access to each other, for exchanging value and for processing data. A "relay chain" coordinates consensus and transaction delivery between member chains. Blockchains are bridged to the Polkadot Nework. This is accomplished with "parachains", which are parallelizable, highly specialized blockchains implemented for each Polkadot participant. Parachains attach to the security provided by the relay chain rather than providing their own.

- [An Introduction to Polkadot](https://blog.stephantual.com/web-three-revisited-part-two-introduction-to-polkadot-what-it-is-what-it-aint-657782051d34)
- [Website](https://polkadot.network/)
- [Polkadot Paper](https://github.com/polkadot-io/polkadotpaper/raw/master/PolkaDotPaper.pdf)(PDF)
- [Overview of "parachain"](https://medium.com/polkadot-network/polkadot-the-parachain-3808040a769a)
- [Now Live: Polkadot POC](https://medium.com/@polkadotnetwork/now-live-polkadot-proof-of-concept-1-3e718512a8d)

## Cosmos Hub

The Cosmos hub connects to zones via IBC (inter-blockchain communication) protocol) and keeps a record of the total number of tokens in each zone. Because all inter-zone transfers go through the Cosmos Hub, you can send tokens from one zone to another without the need for a liquid exchange or trusted third party between zones.

- [Website](https://cosmos.network/intro/hub)
- [Ethermint](https://ethermint.zone/)
- [Introducing the Ethereum Peg Zone](https://blog.cosmos.network/the-internet-of-blockchains-how-cosmos-does-interoperability-starting-with-the-ethereum-peg-zone-8744d4d2bc3f)
- [The Shanghai Accord - Ethereum Scaling Agreement](https://blog.cosmos.network/the-shanghai-accord-ethereum-scaling-agreement-via-cosmos-at-wanxiang-global-blockchain-summit-354efa27b158)

## Loom Interop
- [Announcement of Ethereum, EOS, TRON interop solution](https://medium.com/loom-network/connecting-ethereum-eos-and-tron-making-blockchain-interoperability-a-reality-e5ef6c67716)

## OpenST Mosaic
- [GitHub repo](https://github.com/OpenST/mosaic-contracts)
- [White Paper](https://github.com/OpenST/mosaic-contracts/blob/develop/docs/mosaicv0.pdf)

## Giveth "ghetto bridge"

- [Update mentioning bridge](https://medium.com/giveth/where-are-we-now-status-of-the-giveth-dapp-5f5ba7791d12)

## Grid+ Relay Networks

- [Efficiently Bridging EVM Blockchains](https://blog.gridplus.io/efficiently-bridging-evm-blockchains-8421504e9ced) - discusses designs used in Relay Networks V2

## dogethereum

- [Using Superblocks to Bridge Dogecoin to Ethereum](https://github.com/dogethereum/docs/blob/master/superblocks/superblocks-white-paper.pdf)
- [dogethereum documentation](https://github.com/dogethereum/docs)

## BTC Relay

Ethereum contract for Bitcoin SPV. The main functionality it provides are: verification of a Bitcoin transaction,  optionally relay the Bitcoin transaction to any Ethereum contract storage of Bitcoin block headers, inspection of the latest Bitcoin block header stored in the contract.

- ["btcrelay" GitHub Repo](https://github.com/ethereum/btcrelay)
- [etherscan.io page for 0x41f274c0023f83391de4e0733c609df5a124c3d4](https://etherscan.io/address/0x41f274c0023f83391de4e0733c609df5a124c3d4)

## AltCoin atomic swapping

DEX in which "developers can lock ether tokens in an Ethereum smart contract that specifies the funds will only be sent if an equal amount of bitcoin is sent to a bitcoin address during a specific time window".

- [Altcoin](https://altcoin.io/)
- ["ethatomicswap" GitHub repo](https://github.com/AltCoinExchange/ethatomicswap)
- [Update about atomic swals and plasma](https://blog.altcoin.io/august-update-mobile-ux-atomic-swaps-and-plasma-dex-v2-94680ff9db30) - 9/18/2018 

## Decred atomic swapping

"These tools do not operate solely on-chain. A side-channel is required between each party performing the swap in order to exchange additional data. This side-channel could be as simple as a text chat and copying data."

- On-chain atomic swaps [GitHub Repo](https://github.com/decred/atomicswap)
- [Overview Blog Post](https://blog.decred.org/2017/09/20/On-Chain-Atomic-Swaps/)

## Wanchain atomic swapping

- [Website](https://www.wanchain.org/)
- Wanchain cross-chain contracts [GitHub Repo](https://github.com/wanchain/wanchain-crosschain-contracts)
- [CoinDesk Article](https://www.coindesk.com/wanchains-bridge-to-the-ethereum-blockchain-is-now-open/)

## AION

"This Aion bridging mechanism is an entire Byzantine Fault Tolerant protocol where the majority of nodes a.k.a “Bridge Validators” must agree on transactions or state changes on one network, then pass that transaction to another network to trigger smart contracts."

- [Website](https://aion.network/)
- [reddit discussion](https://www.reddit.com/r/AionNetwork/comments/8gkam6/what_makes_aions_token_swap_with_ethereum_so/dycztsj/)
- [Alpha release Blog Post](https://blog.aion.network/aion-token-bridge-alpha-version-2d3655d9d861)

