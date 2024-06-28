*Overview :-*

MyToken is a simple ERC20-like token implemented in Solidity. It provides basic functionalities such as transferring tokens, minting new tokens, and burning existing tokens. The token has a name and a symbol that can be specified during the deployment of the contract.

*Features:-*

1.Transfer Tokens: Allows users to transfer tokens to other addresses.
2.Mint Tokens: Enables the creation of new tokens.
3.Burn Tokens: Allows the destruction of existing tokens.

*Contract Details:-**

1.Name: The name of the token (e.g., "MyToken").
2.Symbol: The symbol of the token (e.g., "MTK").
3.Total Supply: The total supply of tokens.
4.Balances: A mapping of addresses to their respective balances.

**Events:-**

1.Transfer: Emitted when tokens are transferred from one address to another.
2.Mint: Emitted when new tokens are minted.
3.Burn: Emitted when tokens are burned.

**Functions:-**

1.Constructor-

constructor(string memory _name, string memory _symbol) {
    name = _name;
    symbol = _symbol;
}
*Initializes the contract with a given name and symbol.*


2.transfer

"function transfer(address _to, uint256 _amount) public returns (bool)"

Mints _amount of new tokens to address _to.

Parameters:
_to: The address to mint tokens to.
_amount: The amount of tokens to mint.
burn


function burn(address _from, uint256 _amount) public
Burns _amount of tokens from address _from.

4.Parameters:

_from: The address from which tokens will be burned.
_amount: The amount of tokens to burn.
Example Usage
Deploying the Contract
Deploy the contract with a specified name and symbol.



// Example: Deploying MyToken with name "ExampleToken" and symbol "EXT"
MyToken token = new MyToken("ExampleToken", "EXT");

5.Minting Tokens
*Mint 1000 tokens to a specified address.*


token.mint(0xAbC123..., 1000);

6.Transferring Tokens

*Transfer 100 tokens from the sender's address to another address.*



token.transfer(0xDef456..., 100);

Burning Tokens

*Burn 500 tokens from a specified address.*




token.burn(0xAbC123..., 500);



