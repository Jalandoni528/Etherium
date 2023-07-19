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

     in the second one we would need to do the burn and minting function which is basically the same except using the functions of '+=' on the mint function

in the mint function this will be the increasing of total supply by the amount of that's already passed by using the total supply and balances (with calling the _address and adding the value altgoether) and the address being increased by the balances together with the value.

// burn function
    function burn (address _address, uint _value) public {
        if (balances [_address ] >= _value) {

        totalSupply -= _value;
        balances [_address] -= _value;
        }
        
    }
    recalling from above being a public so it's easier to work with when giving it value, when it's pertaining in real life you would never make it public, knowing the dangers!
The burn function is the inverse of the mint function in that it destroys tokens (much like the mint function, it will accept an address in value) and eliminates the complete supply and balance from the address entirely. Copy and paste the same function, but execute it in the reverse direction by using the subtraction sign while the plus symbol is beneath it, and voilà! You have now received the burn function, which effectively destroys your token!

You'll be utilizing the inverse, '-=' (A quick reminder that any negative integer, such as -1, will never be called in this part, thus the value will always be 0 or above.)


Finally, when the burn function is used, you

# Running the Code
4th thing you'll need to do is deploy and run tab which is located below at the solidity compiler button. with it opening, you'll see the orange button that says deploy which grants you to see if your token is available or not. You'll have to test the waters a.k.a the tokens(abbrv, name, and total supply buttons) within the 'deployed contracts'

lastly and most importantly youll need to copy your account which is directed at the depoly and run transactions and copy paste it and opening the mint and burn below the deployed contracts. Giving them value (equal or greater than the one you're burning) and pasting the account numbers you just got and putting them into the address section and giving value to the value section. When ran by the token abbrv it will give the certain amount of you just did (500 for example to the mint function that will call out and give you 500 tokens as an example) and giving it the total supply of also 500. the same with Burn section, same sequence different number (1000 for example, it will burn the 1k you just gotten to the burn function) and testing it with the totalsupply section and the token abbrv and you're done! that's the whole sequence of mytoken!

# Advice
Any advice can ask @ the discord with Ming/Faith as my guide!

# Authors
Jalandoni, Diosel lei
