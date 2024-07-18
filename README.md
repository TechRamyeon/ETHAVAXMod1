# ETHAVAXMod1

## EMI1 Token Contract

### License
This contract is licensed under the MIT License.

### Contract Description
The EMI1 contract is an ERC20 token contract that inherits from the OpenZeppelin ERC20 and Ownable contracts. It allows for the creation of a custom token with a specified initial supply.

### Constructor
constructor(uint256 initialSupply)
Initializes the contract with a specified initialSupply of tokens.
Sets the token name to "Emiru" and the token symbol to "EMI".
Mints the specified initialSupply of tokens to the contract owner.

### Functions

* ``` mint(address account, uint256 amount) ``` 
* Mints a specified amount of tokens to a specified account.
* Only the contract owner can call this function.
* Requires the amount to be greater than 100.
* Asserts that the account is not the zero address.
* ``` burn(uint256 amount) ```
* Burns a specified amount of tokens from the caller's balance.
* Requires the amount to be greater than zero.
* Requires the caller to have a sufficient balance to burn.
* ``` transfer(address to, uint256 value) ```
* Transfers a specified value of tokens from the caller's balance to a specified to address.
* Requires the to address to be non-zero.
* Requires the caller to have a sufficient balance to transfer.
* Reverts if the transfer would exceed the caller's balance.
