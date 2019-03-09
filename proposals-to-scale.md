
# Scaling the Ethereum Network

Ethereum community proposals to scale, background on scaling in the tech industry, scaling in theory.

## Scaling in General

[Why I love databases](https://medium.com/@jeeyoungk/why-i-love-databases-1d4cc433685f) by Jeeyoung Kim

[How sharding works](https://medium.com/@jeeyoungk/how-sharding-works-b4dec46b3f6) by Jeeyoung Kim

[Making Sense of Ethereum’s Layer 2 Scaling Solutions: State Channels, Plasma, and Truebit](https://medium.com/l4-media/making-sense-of-ethereums-layer-2-scaling-solutions-state-channels-plasma-and-truebit-22cb40dcc2f4)

[Scaling Ethereum in 2018](https://www.youtube.com/watch?v=rnkqMSLuPHA) (video), a presentation by Lane Rettig

## Scaling Blockchains

[Naive to tackle distributed systems and incentive mechanism design separately](https://twitter.com/VladZamfir/status/1014882947781087233) tweet by Vlad Zamfir

[SoK: Consensus in the Age of Blockchains](https://arxiv.org/pdf/1711.03936.pdf) (PDF)

[Scalability of Blockchains Summary of Knowledge](https://github.com/Mechanism-Labs/Summary-of-Knowledge-SoK-Scalability-of-Blockchains/tree/blockchain-stack) - Mechanism Labs paper under development

## General Strategies for Scaling the Ethereum Network

0. Network Bifurcation — separate blockchains (strategies 1–5 directly involve the Ethereum blockchain)

1. Vertical partitioning — endpoints for txn queues, relays,“JSON-RPC APIs”
2. Software optimization — bigger block sizes
3. Network topology optimization
4. Horizontal partitioning via algorithmic sharding — plasmas, state channels, “Layer 2”
5. Horizontal partitioning via dynamic sharding — “Ethereum Sharding”

From [5 Strategies to Scale Ethereum](https://medium.com/@jpitts/5-strategies-to-scale-ethereum-a936ed79b31) by Jamie Pitts

---

## Solutions Available Now

[Spreadsheet summary of scaling solutions](https://docs.google.com/spreadsheets/d/1BQ0bK_LhSQvxtvXryVoIcmxeKMuVJCq6oD0aS5_hpC8/edit#gid=0) - organized by the Web3 Foundation / ScalingNOW initiative

[Lets shard the blockchain using sidechains](https://medium.com/karachain/lets-shard-the-blockchain-using-sidechains-ea42d98b7b28) by Syed Jafar Naqvi

### Raiden Network
- [Description of the developer preview](https://raiden-network.readthedocs.io/en/stable/what_is_the_dev_preview.html)
- [Overview](https://raiden.network/101.html)
- [FAQ](https://raiden.network/faq.html)

### POA Network
- [POA Network](https://poa.network/)
- [Overview](https://github.com/poanetwork/wiki/wiki/What-is-POA)
- [ScalingNOW! Interview 2: on Implementing Parity’s Bridge Chain Solution](https://medium.com/giveth/ethereum-dapp-scaling-poa-network-acee8a51e772) - with Igor & Roman from POA Network

### Loom Network
- [Loom Network](https://loomx.io)
- [Overview](https://medium.com/loom-network/everything-you-need-to-know-about-loom-network-all-in-one-place-updated-regularly-64742bd839fe)
- [Loom.js](https://github.com/loomnetwork/loom-js) - for building browser apps & services that interact with Loom DAppChains 

### Connext Network
- One deployement on mainnet, this is a modified Perun
- [Connext Network](https://connext.network/)
- [Overview of SpankChain live deployment](https://medium.com/connext/our-first-hub-is-live-on-mainnet-b5660486635e)
- [Technical Update 7/27/2018](https://medium.com/connext/connext-v0-4-developer-update-667850e9cdd3)

### SKALE
- Plasma side-chain with an EVM
- [SKALE](https://skalelabs.com/)

### Infura web API
- [Why Infura is the Secret Weapon of Ethereum Infrastructure](https://media.consensys.net/why-infura-is-the-secret-weapon-of-ethereum-infrastructure-af6fc7c77052)
- [Getting started with Infura](https://blog.infura.io/getting-started-with-infura-28e41844cc89)

---

## Under Development / Testnets

Not ready for use in mainnet dapps, but getting closer.



### Matic Network
- Kovan testnet
- [Matic Network](https://matic.network/)
- [Technical Update 9/13/2018](https://medium.com/matic-network/matic-network-technical-update-1-beca0eaa25b4)

### Counterfactual
- [Counterfactual Network](https://counterfactual.com/)
- [Overview](https://medium.com/statechannels/counterfactual-generalized-state-channels-on-ethereum-d38a36d25fc6)
- [Introducing the Force-Move Games Framework](https://medium.com/statechannels/introducing-the-force-move-games-framework-for-state-channels-b32dd953c13f) - collaboration with Magmo

### Cosmos Hub
- [Website](https://cosmos.network/intro/hub)
- [Ethermint](https://ethermint.zone/)
- [Introducing the Ethereum Peg Zone](https://blog.cosmos.network/the-internet-of-blockchains-how-cosmos-does-interoperability-starting-with-the-ethereum-peg-zone-8744d4d2bc3f)
- [The Shanghai Accord - Ethereum Scaling Agreement](https://blog.cosmos.network/the-shanghai-accord-ethereum-scaling-agreement-via-cosmos-at-wanxiang-global-blockchain-summit-354efa27b158)

### Thunder
- [Website](https://www.thundertoken.com/)
- [Thunderella paper](https://eprint.iacr.org/2017/913.pdf) by Elaine Shi and Rafael Pass
- [PAXOS algorithm](https://en.wikipedia.org/wiki/Paxos_(computer_science))

### Polkadot
- [An Introduction to Polkadot](https://blog.stephantual.com/web-three-revisited-part-two-introduction-to-polkadot-what-it-is-what-it-aint-657782051d34)
- [Website](https://polkadot.network/)
- [Polkadot Paper](https://github.com/polkadot-io/polkadotpaper/raw/master/PolkaDotPaper.pdf)(PDF)
- [Now Live: Polkadot POC](https://medium.com/@polkadotnetwork/now-live-polkadot-proof-of-concept-1-3e718512a8d)

---

## Still in R&D

Still being researched, some proof of concept work.

### Plasma Project
- [Plasma Explained](https://medium.com/@argongroup/ethereum-plasma-explained-608720d3c60e)
- [Plasma: Scalable Autonomous Smart Contracts](https://plasma.io/plasma.pdf) (PDF)
- [Minimal Viable Plasma](https://ethresear.ch/t/minimal-viable-plasma/426)

### Ethereum Sharding Project
- [State of Ethereum Protocol #1](https://media.consensys.net/state-of-ethereum-protocol-1-d3211dd0f6) - update from Ben Edgington of PegaSys
- [An engineer's guide to 2.0](https://hackernoon.com/what-to-expect-when-eths-expecting-80cb4951afcd) by James Prestwich
- [How sharding works](https://medium.com/@jeeyoungk/how-sharding-works-b4dec46b3f6)
- [How to Scale Ethereum: Sharding Explained](https://medium.com/prysmatic-labs/how-to-scale-ethereum-sharding-explained-ba2e283b7fce)
- [FAQ](https://github.com/ethereum/wiki/wiki/Sharding-FAQ)
- [Overview and Finality](https://medium.com/@icebearhww/ethereum-sharding-and-finality-65248951f649) by Hsiao-Wei Wang

---

## Research Work

### "snaps" - dapps with SNARKS
- [barryWhiteHat's roll_up](https://github.com/barryWhiteHat/roll_up)
- [Plasma snapp - fully verified plasma chain](https://ethresear.ch/t/plasma-snapp-fully-verified-plasma-chain/3391)

### Virtual Payment Channels
- [Perun Network](https://www.perun.network/)
- [PERUN: Virtual Payment Hubs
over Cryptographic Currencies](https://eprint.iacr.org/2017/635.pdf) (PDF)
- [Foundations of State Channel Networks](https://eprint.iacr.org/2018/320.pdf) (PDF)

---

## What's Happening?

### TrueBit
- [An Introduction to TrueBit](https://medium.com/@simondlr/an-intro-to-truebit-a-scalable-decentralized-computational-court-1475531400c3)
- [Truebit: A scalable verification solution for blockchains](https://people.cs.uchicago.edu/~teutsch/papers/truebit.pdf) (PDF)
- [TrueBit: the marketplace for verifiable computation](https://medium.com/truebit/truebit-the-marketplace-for-verifiable-computation-f51d1726798f) by Sina Habibian

### G-Bridge / ScalingNOW
- [ScalingNOW! Interview 1: Bridge Chains](https://medium.com/giveth/scalingnow-bridge-chains-parity-8c359aca2b01) - with Björn Wagner & Maximilian Krüger from Parity
- [SCLabs ERC-20 -> ERC-777 token bridge](https://github.com/swarmcity/SCLabs-erc20-bridge)
- [G-Bridge Documentation](https://hackmd.io/s/rJDPfbZUG)






