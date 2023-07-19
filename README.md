# ETHAssessment 
This program initializes the very core of using solidity assessment and that is creating a token between all those modules accumulated into one.
# Description
This is a special program that certifies as something evolutionary throughout decades to come and this will be able to help us navigate through the blockchain Ethereum. And by doing so in a most conventional way; Through the world of coding! this serves as a testament that blockchain is the stepping stone beyond the horizon.
# Getting Started
Putting the software together
This is the quickest and most efficient method to learn about Blockchain. Simply navigate to https://remix.ethereum.org/. Then begin with your token! Of course, it's not that simple, is it? Simply tap the addition (+) button and you're ready to code! (with little modifications like as naming your file.sol or whatever you want) ()


This is what I did with mine; it's really simple but can be sorted quickly.

# 1st Code
contract MyToken {

    // public variables here
    string public tokenName = "BETA";
    string public tokenAbbrv = "BTA";
    uint public totalSupply = 0;
You will need to enter variables of your Token name and the Abbreviation of that token being a public domain which will assist you distinguish the Name and the Abbreviations. (As previously indicated, I capitalized 'BETA' and abbreviated it as 'BTA' using all capitals.)

and begin by mapping the variable (creating the Address => uint as your public balances) uint is simply an unsigned int that does not go by negative and also does not contribute anything, therefore being a zero (0) value towards the public variables mentioned in the code.


# 2nd Code
// mapping variable here
    mapping(address => uint) public balances;

    in mapping variables its usually great if its public as it easier to access it entirely.

This will be passing the mapping area and since every address starts with a u end, it will give it to the address and the address will return the token amount that the address has. (therefore its called 'balances')

# 3rd Code

in the mint section, you'll have to do an address and a value that pertains the function that increases the total supply by that number and increases the balance of the address by that amount. Since it has a parameter should have an address and a value (in which i did underscore address and underscore value (_address, _value) to differenciate the parameters into the normal values) and starting with mapping the variable (making the Address => uint as your public balances) uint is simply an unsigned int that doesn't go by negative and also doesn't contribute anything therefore being a zero (0) value towards the public variables stated in the code.
recalling from above being a public so it's easier to work with when giving it value, when it's pertaining in real life you would never make it public, knowing the dangers!

// mint function
    function mint (address _address, uint _value) public {
        totalSupply += _value;
        balances [_address] += _value;
     }
