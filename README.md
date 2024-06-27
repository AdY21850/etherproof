ETH PROOF: Beginner EVM Course Solidity - Metacrafters
This Solidity smart contract, named MyToken, is used to create a basic token. It includes the following features:

Public Variables:
name: A string variable holding the name of the token.
symbol: A string variable containing the symbol or abbreviation of the token.
totalSupply: An unsigned integer variable representing the total supply of the token.
Mapping:
balances: A mapping that associates addresses with token balances, where the address is the key and the balance is the value.
Functions:
constructor: Initializes the token with a name, symbol, and total supply. The total supply is assigned to the contract deployer.
mint: Increases the token's total supply and the balance of a specified address. It requires a valid address and adds the specified amount to the total supply and the balance of the given address.
burn: Decreases the token's total supply and the balance of a specified address. It checks for a valid address and verifies that the address has a sufficient balance before reducing the total supply and the address's balance by the specified amount.
This contract serves as a simple foundation for creating and managing a token on the Ethereum blockchain.
