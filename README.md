# ARRAYS
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
