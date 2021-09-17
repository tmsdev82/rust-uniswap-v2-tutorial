# Uniswap V2 token swap example in Rust

This repository is the completed result for the article on my blog: [TMS Blog - How to swap on Uniswap V2 with Rust Web3](https://tms-dev-blog.com/how-to-swap-on-uniswap-v2-with-rust-web3/). This article describes how to execute a swap transaction of ETH for a token on the Uniswap V2 decentralized exchange.

## Set up 

This project expects certain environment variables to be set. The easiest way is to create a `.env` file containing the following values:

```bash
INFURA_RINKEBY=wss://rinkeby.infura.io/ws/v3/xxxxxxx
PRIVATE_TEST_KEY=xxxxxxxxxxxx
ACCOUNT_ADDRESS=xxxxxxxxxx
```

Where `INFURA_RINKEBY` is an endpoint from your infura.io account. `PRIVATE_TEST_KEY` is a private key from a crypto wallet / account. And, `ACCOUNT_ADDRESS` is a wallet account address.

## Running the project

Caution: running the project with correct configuration will execute a swap of ETH for DAI without asking for confirmation. This example should be run on an Ethereum test network.

```bash
cargo run
```