# Meta Transactions and Executable Signed Txns

Conceived by [Dr. Christian Lundkvist](https://twitter.com/ChrisLundkvist), meta txns enable users to interact with Ethereum without holding any ether.

## uPort
- [Making uPort Smart Contracts Smarter, Part 3: Fixing UX with Meta Txns](https://medium.com/uport/making-uport-smart-contracts-smarter-part-3-fixing-user-experience-with-meta-transactions-105209ed43e0) - Medium article
- [Meta Transaction Relaying Server](https://developer.uport.me/rest-apis/relay-server/)

Jim can use his private key to sign some data and then send this signed data to a relayer (which he has specifically given permission to forward his data). This relayer can then pay the gas for this transaction, and send the data through Jim’s proxy contract.

## Avsa / Executable Signed Transactions
- [The magic of executable signed messages to login and do actions](https://ethereum-magicians.org/t/erc-1077-and-erc-1078-the-magic-of-executable-signed-messages-to-login-and-do-actions/351) - post to the Magicians' Forum by [alexvandesande](https://github.com/alexvandesande)
- [ERC-1077](https://github.com/ethereum/EIPs/pull/1077) - Executable Signed Messages refunded by the contract
- [ERC-1078](https://github.com/ethereum/EIPs/pull/1078) - Log in / signup using ENS subdomains

Allowing users to sign messages to show intent of execution, but allowing a third party relayer to execute them is an emerging pattern being used in many projects. 

## Gnosis Safe
- [Website](https://safe.gnosis.io/)
- [Gnosis Safe contracts](https://github.com/gnosis/safe-contracts)

Aims to provide all users with a convenient, yet secure way to manage their funds and interact with decentralized applications on Ethereum.

## Austin Griffith / metatx.io
- [Bouncer Proxy](https://github.com/austintgriffith/bouncer-proxy)
- [Meta transactions on Ethereum via Identity Proxy Contract](https://www.youtube.com/watch?v=6r3SqCcEVU4&feature=youtu.be) - youtube video

Sandbox for experimenting with etherless meta transactions. The heart of the trick is to sign and recover transactions using Ethereum key pairs both on and off chain.

