# Drift Interface

Drift Interface is a native Solana CPI for the Drift V2 program. This project is written in Rust and is designed to interact with the Drift V2 program on the Solana blockchain.

## Overview

This project provides a native Solana CPI for the Drift V2 program. The IDL is downloaded from the [Drift Labs protocol-v2 repository](https://github.com/drift-labs/protocol-v2/blob/master/sdk/src/idl/drift.json).

## Dependencies

The project relies on the following dependencies:
- **borsh** = "^0.10"
- **num-derive** = "^0.3"
- **num-traits** = "^0.2"
- **serde** (optional) = "^1.0"
- **solana-program** = "^1.16"
- **thiserror** = "^1.0"

## Notes

- This project only works with `solana-program = ^1.16` since it requires `borsh = ^0.10` which introduces the use of const generics in arrays.
- The CPI was generated using [solores](https://github.com/igneous-labs/solores) with some minor fixes by Bulk Labs.

## Usage

To use this CPI, follow these steps:
1. Clone the repository.
2. Build the project using `cargo build`.
3. Refer to the Solana documentation for deploying and interacting with the program.

## Contributing

Contributions are welcome! Please submit a pull request or open an issue to discuss your ideas.

## License

This project is licensed under the MIT License.
