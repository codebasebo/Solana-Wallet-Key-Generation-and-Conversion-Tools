# Solana Wallet Key Generation and Conversion Tools

## Overview
This project provides a set of tools for generating and converting Solana wallet keypairs. It includes functions to:
- Generate new keypairs.
- Convert private keys between Base58 and wallet file formats.
- Load existing wallets from files.

---

## Table of Contents
1. [Features](#features)
2. [Dependencies](#dependencies)
3. [Installation](#installation)
4. [Usage](#usage)
   - [Running Tests](#running-tests)
   - [Generating a New Wallet](#generating-a-new-wallet)
   - [Converting Base58 to Wallet File](#converting-base58-to-wallet-file)
   - [Converting Wallet File to Base58](#converting-wallet-file-to-base58)
5. [Examples](#examples)
6. [Contributing](#contributing)
7. [License](#license)
8. [Contact](#contact)

---

## Features
- **Key Generation**: Generate a new Solana wallet keypair.
- **Base58 Conversion**: Convert a Base58-encoded private key to a wallet file.
- **Wallet File Conversion**: Convert a wallet file byte array to a Base58 string.
- **Loading Wallets**: Load an existing wallet from a JSON file.

---

## Dependencies
- `bs58`: For Base58 encoding and decoding.
- `solana_sdk`: For Solana keypair generation and handling.
- `std::io`: For input/output operations.

---

## Installation

1. **Install Rust and Cargo**:
   Ensure you have Rust and Cargo installed on your system. You can install them from [rust-lang.org](https://www.rust-lang.org/tools/install).

2. **Clone the Repository**:
   ```bash
   git clone https://github.com/codebasebo/Solana-Wallet-Key-Generation-and-Conversion-Tools.git
   
   ```

3. **Build the Project**:
   ```bash
   cargo build
   ```

---

## Usage

### Running Tests
To run the tests, use the following command:
```bash
cargo test
```

---

### Generating a New Wallet
**Test**: `keygen`  
**Description**: Generates a new Solana wallet keypair and prints the public key and the byte representation of the keypair.  
**Usage**:
```bash
cargo test keygen
```

---

### Converting Base58 to Wallet File
**Test**: `base58_to_wallet`  
**Description**: Converts a Base58-encoded private key to a wallet file byte array.  
**Usage**:
1. Run:
   ```bash
   cargo test base58_to_wallet
   ```
2. Input your Base58 private key when prompted.
3. The corresponding wallet file byte array will be printed.

---

### Converting Wallet File to Base58
**Test**: `wallet_to_base58`  
**Description**: Converts a wallet file byte array to a Base58 string.  
**Usage**:
1. Run:
   ```bash
   cargo test wallet_to_base58
   ```
2. Input your wallet file byte array when prompted (e.g., `[1,2,3,...]`).
3. The corresponding Base58 string will be printed.

---

## Examples

### Example 1: Generating a New Wallet
Command:
```bash
cargo test keygen
```
Output:
```
You've generated a new Solana wallet: 7o4VnWjV...
To save your wallet, copy and paste the following into a JSON file:
[174, 47, 154, 16, 202, 193, 206, 113, 199, 190, 53, 133, 169, 175, 31, 56, 222, 53, 138, 189, 224, 216, 117, 173, 10, 149, 53, 45, 73, 251, 237, 246, 15, 185, 186, 82, 177, 240, 148, 69, 241, 227, 167, 80, 141, 89, 240, 121, 121, 35, 172, 247, 68, 251, 226, 218, 48, 63, 176, 109, 168, 89, 238, 135]
```

---

### Example 2: Converting Base58 to Wallet File
Command:
```bash
cargo test base58_to_wallet
```
Input:
```
5HueCGU...
```
Output:
```
Your wallet file is:
[174, 47, 154, 16, 202, 193, 206, 113, 199, 190, 53, 133, 169, 175, 31, 56, 222, 53, 138, 189, 224, 216, 117, 173, 10, 149, 53, 45, 73, 251, 237, 246, 15, 185, 186, 82, 177, 240, 148, 69, 241, 227, 167, 80, 141, 89, 240, 121, 121, 35, 172, 247, 68, 251, 226, 218, 48, 63, 176, 109, 168, 89, 238, 135]
```

---

### Example 3: Converting Wallet File to Base58
Command:
```bash
cargo test wallet_to_base58
```
Input:
```
[174, 47, 154, 16, 202, 193, 206, 113, 199, 190, 53, 133, 169, 175, 31, 56, 222, 53, 138, 189, 224, 216, 117, 173, 10, 149, 53, 45, 73, 251, 237, 246, 15, 185, 186, 82, 177, 240, 148, 69, 241, 227, 167, 80, 141, 89, 240, 121, 121, 35, 172, 247, 68, 251, 226, 218, 48, 63, 176, 109, 168, 89, 238, 135]
```
Output:
```
Your private key in Base58 is:
5HueCGU...
```

---

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes.
4. Push your branch to your forked repository.
5. Submit a pull request.

---

## License
This project is licensed under the [MIT License](LICENSE).

---

## Contact
For questions or feedback, please contact `your_email@example.com`.
```

Let me know if you'd like any further edits!