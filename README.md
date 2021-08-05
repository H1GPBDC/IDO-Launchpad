# IDO Launchpad Token Contract Code (ETH, BSC)
Currency token contract code for IDO Launchpad on Ethereum and Binance Smart Chain blockchain networks. 
# Instructions Before Deployment
Before deployment, make sure to replace the following values accordingly in the solidity files:

For example for ERC20 currency token deployment on Ethereum, replace the following with your desired values in ERC20 Token Ethereum.sol

1. At line 180, replace "YourToken" with your token contract name, e-g IDOToken. So the line will become

        contract IDOToken is ERC20, Ownable {

2. At line 181, replace "TokenName" with your token name and "TokenSymbol" with your currency symbol, e-g "IDO Launchpad" and "IDO". So the line will become 

        constructor () ERC20("IDO Launchpad", "IDO") {
    
3. At line 182, replace TokenSupply with your token maximum supply, e-g for the maximum supply of 500 million tokens, replace with 500000000. So the line will become

        _mint(msg.sender, 500000000 * 10 ** uint(decimals()));

4. Deploy the contract with the name replaced at line 181. Like in the example above, the contract to be deployed on Ethereum blockchain will be IDOToken.

5. Follow the same steps 1 to 4 for BEP20 currency token deployment on Binance Smart Chain, replace the desired values in BEP20 Token Binance Smart Chain.sol
