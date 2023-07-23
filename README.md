## mint_Token

This repository contains a smart contract that implements a basic coin functionality. The contract allows for the creation, destruction, and transfer of tokens. Below are the key features and functions of the contract:

## Contract Details

The contract includes the following public variables to store information about the coin:

- `Bharat`: A string variable that represents the name of the token.
- `Om`: A string variable that represents the abbreviation of the token.
- `totalSupply`: A uint variable that stores the total supply of the token.

## Mapping of Balances

The contract maintains a mapping of addresses to balances. This mapping, named `balances`, associates each address with the number of tokens they hold.

## Mint Function

The contract includes a `mint` function that allows for the creation of new tokens. This function takes two parameters: an address and a value. When called, the `mint` function increases the total supply by the specified value and adds the same amount to the balance of the sender's address.

## Burn Function

The contract also includes a `burn` function that allows for the destruction of tokens. Similar to the `mint` function, the `burn` function takes an address and a value as parameters. When invoked, the `burn` function deducts the specified value from the total supply and reduces the balance of the sender's address accordingly.

## Conditional Checks

The `burn` function includes conditionals to ensure that the balance of the sender is greater than or equal to the amount to be burned. This check prevents the burning of tokens that the sender does not possess, ensuring the integrity of the token system.

## Getting Started

To use this contract, you will need a development environment with Solidity support. You can deploy the contract on a local blockchain network or a testnet. Make sure to set the appropriate values for the token name, abbreviation, and initial supply before deploying the contract.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute the code as per the terms of the license.

## Acknowledgements

This project was inspired by the need for a simple coin contract implementation. Special thanks to the Solidity community for their valuable resources and support.

Please note that this contract is a basic implementation and may not include all the necessary security features for a production-ready token. Use it as a starting point and make the necessary enhancements based on your specific requirements.
