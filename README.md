# MyToken Smart Contract

## Introduction

The MyToken smart contract is an ERC20 token implemented in Solidity for the Ethereum blockchain. This contract provides basic token functionality such as minting, burning, and transferring tokens. Additionally, it inherits from the Ownable contract from OpenZeppelin, allowing for ownership control over the token contract.

## Features

- Initialization with a predefined token supply, assigned to the contract deployer.
- Ability to mint additional tokens to specified addresses by the contract owner.
- Capability to burn tokens from the sender's address.
- Functionality to transfer tokens between addresses.
- Methods to retrieve total token supply and token decimals.

## Dependencies

This contract depends on the OpenZeppelin contracts for ERC20 token functionality and for the Ownable access control.

## Contract Details

### ERC20 Token

- The contract inherits from the ERC20 contract, providing standard token functionality such as transfer, minting, and burning.

### MyToken

- The MyToken contract extends ERC20 and Ownable contracts.
- Upon deployment, the contract initializes with a predefined token supply assigned to the deployer's address.
- The `mintTokens` function allows the contract owner to mint additional tokens to specified addresses.
- The `burnTokens` function enables token holders to burn tokens from their own address.
- Tokens can be transferred between addresses using the `transferTokens` function.
- Additional functions `getTotalSupply` and `getTokenDecimals` provide access to total token supply and token decimals respectively.

## Usage

1. Deploy the MyToken contract to an Ethereum network.
2. Upon deployment, the contract initializes with a predefined token supply.
3. The contract owner can mint additional tokens to specified addresses using the `mintTokens` function.
4. Token holders can burn their tokens using the `burnTokens` function.
5. Tokens can be transferred between addresses using the `transferTokens` function.
6. Users can retrieve total token supply and token decimals using the provided functions.

## License

This code is released under the MIT License. See the provided `LICENSE` file for details.
