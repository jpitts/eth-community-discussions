
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

## Ethereum Roadmap

[A rollup-centric ethereum roadmap](https://ethereum-magicians.org/t/a-rollup-centric-ethereum-roadmap/4698) by Vitalik Buterin, Oct. 2020

"the Ethereum ecosystem is likely to be all-in on rollups (plus some plasma and channels) as a scaling strategy for the near and mid-term future"

[Lets shard the blockchain using sidechains](https://medium.com/karachain/lets-shard-the-blockchain-using-sidechains-ea42d98b7b28) by Syed Jafar Naqvi

## General Strategies for Scaling the Ethereum Network

0. Network Bifurcation — separate blockchains (strategies 1–5 directly involve the Ethereum blockchain)

1. Vertical partitioning — endpoints for txn queues, relays,“JSON-RPC APIs”
2. Software optimization — bigger block sizes
3. Network topology optimization
4. Horizontal partitioning via algorithmic sharding — plasmas, state channels, “Layer 2”
5. Horizontal partitioning via dynamic sharding — “Ethereum Sharding”

From [5 Strategies to Scale Ethereum](https://medium.com/@jpitts/5-strategies-to-scale-ethereum-a936ed79b31) by Jamie Pitts

---

## Retro or Bootstrap Scaling Solutions

### Infura web API - gateway to Ethereum and other networks
- [Why Infura is the Secret Weapon of Ethereum Infrastructure](https://media.consensys.net/why-infura-is-the-secret-weapon-of-ethereum-infrastructure-af6fc7c77052)
- [Getting started with Infura](https://blog.infura.io/getting-started-with-infura-28e41844cc89)

---

## L2s and Side Chains Available Now

[Spreadsheet summary of scaling solutions](https://docs.google.com/spreadsheets/d/1BQ0bK_LhSQvxtvXryVoIcmxeKMuVJCq6oD0aS5_hpC8/edit#gid=0) - organized by the Web3 Foundation / ScalingNOW initiative

### Loopring
- ZK Rollups
- [Loopring](https://loopring.org/#/)
- [Overview](https://loopring.readthedocs.io/en/latest/English/overview/)
- [2020 Roadmap](https://loopring.org/#/post/loopring-2020-development-roadmap)
- Deployed system is [Loopring](https://loopring.org/#/) itself

### Starkware
- ZK Rollups
- [StarkEx Website](https://starkware.co/product/starkex/)
- Deployed systems: [DeversiFi](https://www.deversifi.com/)

### zkSync
- ZK Rollups
- [zkSync](https://zksync.io/)
- [Documentation](https://zksync.io/dev/)
- [Overview](https://medium.com/matter-labs/zksync-is-live-bringing-trustless-scalable-payments-to-ethereum-9c634b3e6823)
- Deployed systems: [zkSync Wallet](https://wallet.zksync.io/)

### SKALE
- Plasma L2 w/ an EVM
- [SKALE](https://skalelabs.com/)
- [Why SKALE?](https://medium.com/skale/why-skale-de649cbf3ab9) - Overview
- Deployed systems: 

### Matic Network
- Plasma L2 w/ an EVM
- [Matic Network](https://matic.network/)
- [Matic 2019 Year In Review](https://medium.com/matic-network/year-in-review-2019-matic-network-aa47bf1b201b)
- Deployed systems: [Quickswap](https://quickswap.exchange/#/swap)

### Connext Network
- State channels
- [Connext Network](https://connext.network/)
- [Overview of SpankChain live deployment](https://medium.com/connext/our-first-hub-is-live-on-mainnet-b5660486635e)
- [Overview of v2.0 on mainnet](https://medium.com/connext/connext-v2-0-is-on-mainnet-b818864d3687)

### Raiden Network
- State Channels
- [Description of the developer preview](https://raiden-network.readthedocs.io/en/stable/what_is_the_dev_preview.html)
- [Overview](https://raiden.network/101.html)
- [FAQ](https://raiden.network/faq.html)

### Counterfactual
- State Channels
- [Counterfactual Network](https://counterfactual.com/)
- [Overview](https://medium.com/statechannels/counterfactual-generalized-state-channels-on-ethereum-d38a36d25fc6)
- [Introducing the Force-Move Games Framework](https://medium.com/statechannels/introducing-the-force-move-games-framework-for-state-channels-b32dd953c13f) - collaboration with Magmo

### POA Network
- Side Chain w/ an EVM
- [POA Network](https://poa.network/)
- [Overview](https://github.com/poanetwork/wiki/wiki/What-is-POA)
- [ScalingNOW! Interview 2: on Implementing Parity’s Bridge Chain Solution](https://medium.com/giveth/ethereum-dapp-scaling-poa-network-acee8a51e772) - with Igor & Roman from POA Network
- Deployed systems: [xDAI Chain](https://www.xdaichain.com/), [Burner Wallet](https://xdai.io/)

---

## L1s that bridge to Ethereum mainnet

### Cosmos Hub
- L1 w/ bridge to Ethereum mainnet
- [Website](https://cosmos.network/intro/hub)
- [Ethermint](https://ethermint.zone/) - under [active development](https://github.com/ChainSafe/ethermint) by ChainSafe
- [Introducing the Ethereum Peg Zone](https://blog.cosmos.network/the-internet-of-blockchains-how-cosmos-does-interoperability-starting-with-the-ethereum-peg-zone-8744d4d2bc3f)
- [The Shanghai Accord - Ethereum Scaling Agreement](https://blog.cosmos.network/the-shanghai-accord-ethereum-scaling-agreement-via-cosmos-at-wanxiang-global-blockchain-summit-354efa27b158)

### Polkadot
- L1 w/ bridge to Ethereum mainnet
- [An Introduction to Polkadot](https://blog.stephantual.com/web-three-revisited-part-two-introduction-to-polkadot-what-it-is-what-it-aint-657782051d34)
- [Website](https://polkadot.network/)
- [Polkadot Paper](https://github.com/polkadot-io/polkadotpaper/raw/master/PolkaDotPaper.pdf)(PDF)
- [Now Live: Polkadot POC](https://medium.com/@polkadotnetwork/now-live-polkadot-proof-of-concept-1-3e718512a8d)


---

## Under Development / Testnets

Not ready for use w/ mainnet Ethereum dapps, but getting closer.

### Eth2 Phase 0
- Phase 0 is the Beacon chain, used for protocol attestations
- Will be useful because it can support solutions based on Optimistic Rollups
- [Phase 0 Specification](https://github.com/ethereum/eth2.0-specs) and [Implementations](https://docs.ethhub.io/ethereum-roadmap/ethereum-2.0/eth2.0-teams/teams-building-eth2.0/) 

### Optimism
- Optimistic Rollups w/ EVM
- [Optimism](https://optimism.io/)
- [OVM deep-dive](https://medium.com/ethereum-optimism/ovm-deep-dive-a300d1085f52)

### Hermez
- ZK Rollups
- [Hermez](https://hermez.io/)
- [White Paper](https://hermez.io/hermez-whitepaper.pdf)

### Fuel Labs
- Optimistic Rollups
- [Fuel Labs](https://fuel.sh/)
- [Overview of beta / testnet](https://medium.com/@fuellabs/announcing-the-fuel-v0-open-beta-565a2d340fc3)

### Aztec 2.0
- ZK Rollups w/ privacy
- [Aztec](https://aztec.network/)
- [Overview of Aztec 2.0](https://medium.com/aztec-protocol/aztec-zkrollup-layer-2-privacy-1978e90ee3b6)

### Tiramisu
- Optimistic Rollups
- [Project Repo](https://github.com/dharma-eng/Tiramisu)
- [Overview / design principles](https://github.com/dharma-eng/Tiramisu/blob/master/docs/README.md#overview)

### Plasma Chamber
- OVM over Plasma Cashflow
- [Cryptoeconomics Lab's Plasma Chamber](https://www.cryptoeconomicslab.com)
- [Overview](https://github.com/cryptoeconomicslab/plasma-chamber) and [Documentation](https://github.com/cryptoeconomicslab/plasma-chamber/wiki)

### Plasm
- OVM on Substrate / Polkadot
- [Project Repo](https://github.com/staketechnologies/Plasm)
- [White Paper](https://github.com/staketechnologies/plasmdocs/blob/master/wp/en.pdf)

---

## Still in R&D / Prototypes

### Eth2 / Ethereum Sharding Project - Phase 1 and 2, General Protocol
- Note: Phase 0 is specified, viable clients are built, and the network will be launching in the near future
- [Phase 1](https://docs.ethhub.io/ethereum-roadmap/ethereum-2.0/eth-2.0-phases/#phase-1-shard-chains) shards and [Phase 2](https://docs.ethhub.io/ethereum-roadmap/ethereum-2.0/eth-2.0-phases/#phase-2-state-execution) execution engines
- [An engineer's guide to 2.0](https://hackernoon.com/what-to-expect-when-eths-expecting-80cb4951afcd) by James Prestwich
- [How sharding works](https://medium.com/@jeeyoungk/how-sharding-works-b4dec46b3f6)
- [How to Scale Ethereum: Sharding Explained](https://medium.com/prysmatic-labs/how-to-scale-ethereum-sharding-explained-ba2e283b7fce)
- [FAQ](https://github.com/ethereum/wiki/wiki/Sharding-FAQ)
- [Overview and Finality](https://medium.com/@icebearhww/ethereum-sharding-and-finality-65248951f649) by Hsiao-Wei Wang

### Nitro Protocol
- "standard" state channels
- [Nitro Protocol](https://protocol.statechannels.org)
- [Documentation](https://protocol.statechannels.org/docs/state-channels/overview)

### Smart Contracts and "compute" in Filecoin
- [Filecoin WP - July 19, 2017](https://filecoin.io/filecoin.pdf) @ Section 7.1 "Contracts in Filecoin"
- [Filecoin: protocol overview - BPASE '18](https://www.youtube.com/watch?v=vyRZBeMtkrA) @ 21:57

---

## Research Work

### Ethereum Community R&D
- [EthResearch](https://ethresear.ch/) is where discussions about scaling Ethereum generally happen

### Stateless Ethereum / Eth1x
- [EthResearch topics](https://ethresear.ch/c/eth1x-research)

### State Channels
- [Overview of state channels](https://docs.ethhub.io/ethereum-roadmap/layer-2-scaling/state-channels/)
- [Proposed state channels standard](https://statechannels.org)

### Plasma Framework
- [Plasma Explained](https://medium.com/@argongroup/ethereum-plasma-explained-608720d3c60e)
- [Plasma World Map](https://ethresear.ch/t/plasma-world-map-the-hitchhiker-s-guide-to-the-plasma/4333)
- [Minimal Viable Plasma](https://ethresear.ch/t/minimal-viable-plasma/426)

### Rollups
- [Summary: The Dawn of Hybrid Layer 2 Protocols](https://vitalik.ca/general/2019/08/28/hybrid_layer_2.html) - by Vitalik Buterin

**Optimistic Rollups**
- [Minimal Viable Merged Consensus](https://ethresear.ch/t/minimal-viable-merged-consensus/5617) - by John Adler and Mikerah Quintyne-Collins
- [The Whys of Optimistic Rollup](https://medium.com/@adlerjohn/the-why-s-of-optimistic-rollup-7c6a22cbb61a)

**ZK-Rollups**
- [On-chain scaling to potentially ~500 tx/sec through mass tx validation](https://ethresear.ch/t/on-chain-scaling-to-potentially-500-tx-sec-through-mass-tx-validation/3477) - by Vitalik Buterin
- [barryWhiteHat's roll_up](https://github.com/barryWhiteHat/roll_up)
- [Plasma snapp - fully verified plasma chain](https://ethresear.ch/t/plasma-snapp-fully-verified-plasma-chain/3391)

### Virtual Payment Channels
- [Perun Network](https://www.perun.network/)
- [PERUN: Virtual Payment Hubs
over Cryptographic Currencies](https://eprint.iacr.org/2017/635.pdf) (PDF)
- [Foundations of State Channel Networks](https://eprint.iacr.org/2018/320.pdf) (PDF)

---

## Reddit's Scaling Bake-off Submissions

[NEAR Protocol team submission](https://www.reddit.com/r/ethereum/comments/i1b4b3/nears_submission_to_reddits_scaling_bakeoff/)

[Raiden team submission](https://www.reddit.com/r/ethereum/comments/hbjx25/the_great_reddit_scaling_bakeoff/fzwd8o3/)

[OMG Network team submission](https://www.reddit.com/r/ethereum/comments/i19us9/omg_networks_great_reddit_scaling_bakeoff_proposal/)

[Fuel Labs team submission](https://www.reddit.com/r/ethereum/comments/i1cimc/the_great_reddit_scaling_bakeoff_submission_by/)

[Celer Network team submission](https://www.reddit.com/r/ethereum/comments/i2hx80/celer_joins_reddit_great_scaling_bakeoff_exactly/)

[Connect / Spacefold team submission](https://www.reddit.com/r/ethereum/comments/i1eooc/spacefold_connexts_submission_to_the_great_reddit/)

---

## Recently Reoriented

### LeapDAO / Plasma
- A set of NFTs represents verifiable EVM state transitions, enabling the EVM to "leap" into Plasma 
- [Plasma Leap white paper](https://docs.google.com/document/d/1vStTjqvqZGyiI5AVtpwCIMlHFnzC_4bbixsCfs27-M8/edit#heading=h.krdzwa9n8mii)
- [Documentation](https://docs.leapdao.org)
- [Announcement of reorientation](http://ipfs.leapdao.org/blog/mainnet-shutdown) - moving toward ORUs and ZK-rollups

### Matter Labs / Plasma
- SNARKs-driven Plasma
- [Matter Labs](https://matter-labs.io/)
- [Introducing Matter testnet](https://medium.com/matter-labs/introducing-matter-testnet-502fab5a6f17)
- [Announcement of reorientation](https://medium.com/matter-labs/software-engineering-jobs-at-matter-labs-c456d01b2a02) - moved toward ZK-rollups

### Plasma Group
- generalized framework for all Plasma types
- [Documentation](https://docs.plasma.group/projects/spec/en/latest/)
- [Announcement of reorientation](https://medium.com/plasma-group/on-to-new-beginnings-e9d76b170752) - moved toward ORUs, group is re-named to Optimism

---

## Abandoned / What's Happening?

Recently not enough information, GitHub updates, etc. to determine status

### ThunderCore
- [Website](https://www.thundertoken.com/)
- [Thunderella paper](https://eprint.iacr.org/2017/913.pdf) by Elaine Shi and Rafael Pass
- [PAXOS algorithm](https://en.wikipedia.org/wiki/Paxos_(computer_science))

### Loom Network
- "Looks like the Loom Network has thrown in the towel" - 5/20/2020 [CoinTelegraph article](https://cointelegraph.com/news/looks-like-the-loom-network-has-thrown-in-the-towel)
- "We haven't gone anywhere, and the chain is still operational." - 5/20/2020 [Tweet from @LoomNetwork](https://twitter.com/loomnetwork/status/1259328823218192385)
- [Loom Network](https://loomx.io)
- [Overview](https://medium.com/loom-network/everything-you-need-to-know-about-loom-network-all-in-one-place-updated-regularly-64742bd839fe)
- [Loom.js](https://github.com/loomnetwork/loom-js) - for building browser apps & services that interact with Loom DAppChains 

### TrueBit
- [An Introduction to TrueBit](https://medium.com/@simondlr/an-intro-to-truebit-a-scalable-decentralized-computational-court-1475531400c3)
- [Truebit: A scalable verification solution for blockchains](https://people.cs.uchicago.edu/~teutsch/papers/truebit.pdf) (PDF)
- [TrueBit: the marketplace for verifiable computation](https://medium.com/truebit/truebit-the-marketplace-for-verifiable-computation-f51d1726798f) by Sina Habibian

### G-Bridge / ScalingNOW
- [ScalingNOW! Interview 1: Bridge Chains](https://medium.com/giveth/scalingnow-bridge-chains-parity-8c359aca2b01) - with Björn Wagner & Maximilian Krüger from Parity
- [SCLabs ERC-20 -> ERC-777 token bridge](https://github.com/swarmcity/SCLabs-erc20-bridge)
- [G-Bridge Documentation](https://hackmd.io/s/rJDPfbZUG)






