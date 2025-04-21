# Single Offer Token Exchange

A smart contract built on the Soroban platform that facilitates token pair trading between a single seller and multiple buyers.

## Contract

ℹ️  Skipping install because wasm already installed
ℹ️  Using wasm hash 84571eb25a7fd4c3d1916d92044b7a50ea04f98b5d80624bedfc09d86bb50483
ℹ️  Simulating deploy transaction…
ℹ️  Transaction hash is eba1bb2a3517c8d09e6bb97199c809d0c542242c99fbee63dc4cfe3c9202bf11
🔗 https://stellar.expert/explorer/testnet/tx/eba1bb2a3517c8d09e6bb97199c809d0c542242c99fbee63dc4cfe3c9202bf11
ℹ️  Signing transaction: eba1bb2a3517c8d09e6bb97199c809d0c542242c99fbee63dc4cfe3c9202bf11
🌎 Submitting deploy transaction…
🔗 https://stellar.expert/explorer/testnet/contract/CBTZ34PLRVBVTVA6BYYOQF4KBDSOVSWTI34DQHY6S6IWDYKXRTWPFUQV
✅ Deployed!
CBTZ34PLRVBVTVA6BYYOQF4KBDSOVSWTI34DQHY6S6IWDYKXRTWPFUQV


## Overview

This contract implements a simple yet effective token exchange mechanism where a seller can create an offer to exchange one token for another at a specified price ratio. Multiple buyers can then trade with this offer without the need for order matching or complex exchange logic.

## Features

- **Single Seller Model**: One seller can create an offer for multiple buyers
- **Fixed Price Ratio**: Trading occurs at a predetermined price ratio
- **Minimum Amount Protection**: Buyers can specify a minimum amount to receive
- **Price Updates**: Seller can update the price ratio as needed
- **Withdrawal Function**: Seller can withdraw tokens from the contract

## Contract Structure

### Data Structures

- **DataKey**: Defines storage keys used in the contract
  - `Offer`: Stores the offer information

- **Offer**: Contains all the details about the trading offer
  - `seller`: Address of the seller
  - `sell_token`: Address of the token being sold
  - `buy_token`: Address of the token being bought
  - `sell_price`: Unit price for selling (per token)
  - `buy_price`: Unit price for buying (per token)

## Technical Details

- Built using the Soroban SDK for Stellar's smart contract platform
- Implemented with `#![no_std]` for efficient operation in blockchain environments
- Uses Rust's type system for safety and reliability
- Simple storage model with a single offer state

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
