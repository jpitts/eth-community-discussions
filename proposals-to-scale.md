
# Scaling the Ethereum Network

Ethereum community proposals to scale, background on scaling in the tech industry, scaling in theory.

## Scaling in General

[Why I love databases](https://medium.com/@jeeyoungk/why-i-love-databases-1d4cc433685f) by Jeeyoung Kim

[How sharding works](https://medium.com/@jeeyoungk/how-sharding-works-b4dec46b3f6) by Jeeyoung Kim

[Making Sense of Ethereum’s Layer 2 Scaling Solutions: State Channels, Plasma, and Truebit](https://medium.com/l4-media/making-sense-of-ethereums-layer-2-scaling-solutions-state-channels-plasma-and-truebit-22cb40dcc2f4)

[Scaling Ethereum in 2018](https://www.youtube.com/watch?v=rnkqMSLuPHA)(youtube), a presentation by Lane Rettig

## General Strategies for Scaling the Ethereum Network

Vitalik Buterin [tweet-replied](https://twitter.com/VitalikButerin/status/1005384496311496704):

> My view: there are basically 5 scaling strategies:
> 1. Many separate chains
> 2. Super-big blocks
> 3. Incremental improvements that don't change security model (eg. replacing txs + sigs with compressed delta + STARKs)
> 4. Layer 2 (channels and plasma)
> 5. Sharding

Jamie Pitts [tweet-replied](https://twitter.com/jamiepitts/status/1005949301502033921):

> Basic strategies for scaling Ethereum:
> 1. Bifurcation - sep. chains
> 2. Vert. partitioning - big blocks, SMR
> 3. Software optimization
> 4. Network topology optimization
> 5. Horiz. partitioning - algorithmic sharding
> 6. Horiz. partitioning - dynamic sharding

Strategies 2-6 can be seen as involving a single chain, even though all chains will eventually interconnect. Strategy 4 with its channels and plasmas and verified offloading may additionally be categorized as bifurcation, though involving far more integration than 1.

Added #4 due to [a suggestion by @DisruptionJoe](https://twitter.com/DisruptionJoe/status/1005818278382620672).

---

## Solutions Available Now

[Spreadsheet summary of scaling solutions](https://docs.google.com/spreadsheets/d/1BQ0bK_LhSQvxtvXryVoIcmxeKMuVJCq6oD0aS5_hpC8/edit#gid=0) - organized by the Web3 Foundation / ScalingNOW initiative

[Lets shard the blockchain using sidechains](https://medium.com/karachain/lets-shard-the-blockchain-using-sidechains-ea42d98b7b28) by Syed Jafar Naqvi

### G-Bridge / ScalingNOW
- [ScalingNOW! Interview 1: Bridge Chains](https://medium.com/giveth/scalingnow-bridge-chains-parity-8c359aca2b01) - with Björn Wagner & Maximilian Krüger from Parity
- [SCLabs ERC-20 -> ERC-777 token bridge](https://github.com/swarmcity/SCLabs-erc20-bridge)
- [G-Bridge Documentation](https://hackmd.io/s/rJDPfbZUG)

### Raiden developer preview
- [Description of the developer preview](https://raiden-network.readthedocs.io/en/stable/what_is_the_dev_preview.html)
- [Overview](https://raiden.network/101.html)
- [FAQ](https://raiden.network/faq.html)

### Infura web API
- [Why Infura is the Secret Weapon of Ethereum Infrastructure](https://media.consensys.net/why-infura-is-the-secret-weapon-of-ethereum-infrastructure-af6fc7c77052)
- [Getting started with Infura](https://blog.infura.io/getting-started-with-infura-28e41844cc89)

---

## Under Development / Testnets

Not ready for use in mainnet dapps, but getting closer.

### POA Network
- [Website](https://poa.network/)
- [POA Network overview](https://github.com/poanetwork/wiki/wiki/What-is-POA)
- [ScalingNOW! Interview 2: on Implementing Parity’s Bridge Chain Solution](https://medium.com/giveth/ethereum-dapp-scaling-poa-network-acee8a51e772) - with Igor & Roman from POA Network

### Cosmos Hub
- [Website](https://cosmos.network/intro/hub)
- [Ethermint](https://ethermint.zone/)
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

### TrueBit
- [An Introduction to TrueBit](https://medium.com/@simondlr/an-intro-to-truebit-a-scalable-decentralized-computational-court-1475531400c3)
- [Truebit: A scalable verification solution for blockchains](https://people.cs.uchicago.edu/~teutsch/papers/truebit.pdf) (PDF)
- [TrueBit: the marketplace for verifiable computation](https://medium.com/truebit/truebit-the-marketplace-for-verifiable-computation-f51d1726798f) by Sina Habibian

---

## Still in R&D

Still being researched, some proof of concept work.

### Plasma Project
- [Plasma Explained](https://medium.com/@argongroup/ethereum-plasma-explained-608720d3c60e)
- [Plasma: Scalable Autonomous Smart Contracts](https://plasma.io/plasma.pdf) (PDF)
- [Minimal Viable Plasma](https://ethresear.ch/t/minimal-viable-plasma/426)

### Ethereum Sharding Project
- [How sharding works](https://medium.com/@jeeyoungk/how-sharding-works-b4dec46b3f6)
- [How to Scale Ethereum: Sharding Explained](https://medium.com/prysmatic-labs/how-to-scale-ethereum-sharding-explained-ba2e283b7fce)
- [FAQ](https://github.com/ethereum/wiki/wiki/Sharding-FAQ)
- [Overview and Finality](https://medium.com/@icebearhww/ethereum-sharding-and-finality-65248951f649) by Hsiao-Wei Wang

---

## Research Work

### Virtual Payment Channels

- [PERUN: Virtual Payment Hubs
over Cryptographic Currencies](https://eprint.iacr.org/2017/635.pdf) (PDF)
- [Foundations of State Channel Networks](https://eprint.iacr.org/2018/320.pdf) (PDF)






