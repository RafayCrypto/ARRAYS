# ARRAYS and STRUCT
a simple array concept of solidity so that bunch of orders can be stored for a particular coin

// SPDX-License-Identifier: MIT
// SPDX-License-Identifier: MIT
pragma solidity  ^0.8.13;

contract  ARRAYS {

    uint public num = 1;

    uint[] public number;

    function addingElement(uint NO) public 
    {
        number.push(NO);
    }

    function size() public returns (uint)
    {
        return number.length;

    }

    function remove(uint index) public 
    {
        delete number[index];
    }

    
}


_______________

# struct here
A struct is just like a template function or also generics like where a data type is already predefined and you can call all the required datatypes variables in just a single function

pragma solidity ^0.7.5;

contract team
{
    uint public number = 1;

    Player[] public players;

    struct Player
    {
        string firstName;
        string lastName;
        uint age;
    }

    function addPlayer(string memory _firstName, string memory _lastName, uint age ) public 
    {
        players.push(Player(_firstName, _lastName, age));
    }

}
