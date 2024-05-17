# DIAZ TOKEN
The Ethereum blockchain uses the computer language Solidity to create smart contracts. A digital asset that is generated and exchanged on a 
blockchain. Solidity tokens are virtual goods that are implemented as smart contracts on the Ethereum blockchain and made with the Solidity programming language.

## Description
In a decentralized system, Solidity tokens can be utilized for a number of things, such as reward systems, governance, and payment methods. 
program (dApp). Decentralized exchanges (DEXs) allow for their trading, and their attributes and features might vary widely based on 
the way they're coded.

### Executing program
Remix is an online Solidity IDE that may be used to run this software; to get started, visit the Remix website at https://remix.ethereum.org.

Select the "Solidity Compiler" tab from the sidebar on the left to begin compiling the code. Make sure "0.8.18(" is selected under the "Compiler" option.
or an alternative version that is compatible), and then select the "Compile token" option.

code blocks for commands

```
//SPDX-License-Identifier: MIT
pragma solidity ^0.8.18;

contract MyToken {


    string public tokenName = "Diaz";
    string public tokenAbbrv = "Joshua";
    uint public TotalSupply = 0;

mapping(address => uint) public balances;


function mint (address _address, uint _value) public {
       TotalSupply += _value;
       balances[_address] += _value;
}

function burn (address _address, uint _value) public {
       if (balances[_address] >= _value) {
       TotalSupply -= _value;
       balances[_address] -= _value;
       }
    }
}

```
To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.18(
or another compatible version), and then click on the "Compile project.sol" button.

After compiling the code, you can deploy the contract by selecting the "Deploy & Run Transactions" tab in the left-hand sidebar. Click the "Deploy" button.

after i deploy it im going to deployed contracts then copy the ACCOUNT 

*click down the mint tab then paste the account and i put my desired token ammount(100000)then click transact to confirm the token amount that i 
inserted i click the totalsupply below of TokenName

to test the burn function
*click down the burn tab then paste the account and i put my desire amount that will be burn (50000) then click transact to confirm it again how much
token i had left i click the totalsupply.

last to check if the IF STATEMENT i made is working im going to put 25000 for the amount to be burn then testing if it will burn the token more than i have
as u expected nothings happen bacause my system cannot burn token more than i have.

## Authors

Joshua D. Diaz
@Joshuadaccadiaz


## License

This project is licensed under the MIT License - see the LICENSE.md file for details



