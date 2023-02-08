# Developing on Near Workshop: University of Waterloo (Feb 2023)

## Setup

To prepare for the workshop, please complete the following steps.
This will set up your development enviornment, allowing you to participate in the workshop.

1. Ensure `git` is installed. I do not recommend doing development work on Windows (if you are doing this then I think WSL is the way to go), and most non-Windows OSs come with `git` pre-installed, but in case you don't have it then definitely get it.
2. Install Rust. Follow the instructions on the [Rust website](https://www.rust-lang.org/tools/install).
3. Clone this repository: `git clone https://github.com/birchmd/waterloo-bc-workshop-2023.git`. From this point forward, assume commands are run from the repository's directory.
4. Install `cargo-near`: `cargo install cargo-near`. If you're curious about what this is, see the [cargo-near repository](https://github.com/near/cargo-near) for more information.
5. Install the Wasm compilation target for Rust: `rustup target add wasm32-unknown-unknown`.
6. Try building the contract in this repository with `cargo near build`. If you are having problems with this be sure to raise it with me during the workshop.
7. Create an account on Near's testnet. Follow the instructions on the [Near Wallet website](https://wallet.testnet.near.org/create). Choose the "Secure Passphrase" option and be sure to keep the generated passphrase handy. You don't need to worry too much about keeping it a secure place since this is only for testnet. I will reference the name of this account as `$MY_ACCOUNT` through the remaining instructions.
8. Install `near-cli`. There is a convenience script to do this in this repository (Unix platforms only) `./install_near_cli.rs`. If you want more information about the `near-cli` tool, see [its repository](https://github.com/near/near-cli).
9. Login to `$MY_ACCOUNT` with `near-cli`. Use the command `./near login` and follow the instructions.
10. Create a sub-account of `$MY_ACCOUNT` to deploy the contract to: `./near --masterAccount $MY_ACCOUNT create-account --initialBalance 50 chat.$MY_ACCOUNT`

## Deploying and interacting with the contract

TODO
