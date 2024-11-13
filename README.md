# Soltrac

Soltrac is a command-line interface (CLI) tool designed to copytrade a Solana wallet. It monitors transactions of a specified wallet and replicates them. Please note that this project is still under development and not fully functional yet.

## Features

- Monitors a specified Solana wallet for new transactions.
- Processes transactions involving Raydium and Jupiter swaps.
- Recognizes transactions from Raydium and Jupiter.
- Planned support for pump.fun transactions.

## Installation

To install Soltrac, you need to have Rust and Cargo installed. If you don't have them installed, you can follow the instructions [here](https://www.rust-lang.org/tools/install).

Clone the repository and navigate to the project directory:

```sh
git clone https://github.com/joaquinsoza/soltrac.git
cd soltrac
```

## Usage

To run Soltrac, use the following command in your terminal:

```sh
cargo run --release -- copytrade <WALLET_ADDRESS>
```

Replace `<WALLET_ADDRESS>` with the address of the wallet you want to copytrade. Note that you need to use Solana CLI to read the keypair from there to be used.

## Example

```sh
cargo run --release -- copytrade 3M5tY7J8z9Q1a2b3c4d5e6f7g8h9i0j1k2l3m4n5o6p7
```

This command will start monitoring the specified wallet for new transactions and replicate them as they are detected.

## Current Status

Currently, Soltrac can recognize if a transaction is from Raydium or Jupiter when a Solana address is provided. Work is ongoing to support transaction parsing and interpretation, starting with Raydium transactions.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## Author

Soltrac is developed by coderipper.
