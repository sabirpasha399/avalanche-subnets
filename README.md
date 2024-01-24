#  Vault Contract

## Overview

The Vault contract is a simple implementation in Solidity that represents a basic vault for handling deposits and withdrawals of an ERC-20 token. It is designed to be used with any ERC-20 compliant token.

## Smart Contracts

### Vault.sol

This contract defines the Vault, which holds an ERC-20 token and allows users to deposit and withdraw funds. The contract uses a simple calculation to mint and burn shares based on the amount of tokens deposited or withdrawn. The main functions include:

- `deposit(uint _amount) external`: Allows users to deposit ERC-20 tokens into the vault, minting shares in return.
  
- `withdraw(uint _shares) external`: Allows users to withdraw ERC-20 tokens from the vault, burning the corresponding shares.

### IERC20.sol

This is an interface representing the ERC-20 standard functions. It provides a blueprint for any ERC-20 token to be used with the Vault contract.

## Usage

To use the Vault contract:

1. Deploy the ERC-20 token contract.
2. Deploy the Vault contract, passing the address of the ERC-20 token as a constructor argument.
3. Users can then interact with the Vault contract to deposit and withdraw tokens.

Make sure to have sufficient allowances set for the Vault contract to transfer tokens on behalf of the user.

## Security Considerations

- Ensure that the deployed ERC-20 token is correctly implemented and adheres to the ERC-20 standard.
- Review and test the Vault contract thoroughly before deploying it in a production environment.


#  ERC20 Contract

## Overview

The ERC20 contract is a basic implementation of the ERC-20 token standard in Solidity. It allows for the creation of a custom token with functionalities like transfers, approvals, and allowances.

## Smart Contract

### ERC20.sol

This contract defines the ERC-20 token. It includes standard functions such as:

- `transfer(address recipient, uint amount) external`: Transfers tokens from the sender's account to the recipient's account.

- `approve(address spender, uint amount) external`: Approves the spender to spend a certain amount of tokens on behalf of the owner.

- `transferFrom(address sender, address recipient, uint amount) external`: Transfers tokens from one account to another, given approval from the sender.

- `mint(uint amount) external`: Mints new tokens and adds them to the total supply.

- `burn(uint amount) external`: Burns tokens, reducing the total supply.

## Usage

To use the ERC20 contract:

1. Deploy the ERC20 contract.
2. Interact with the contract to transfer tokens, approve spending, and mint or burn tokens.

## Author 

Sabir pasha

pashasabir399@gmail.com
