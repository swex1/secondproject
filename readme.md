<!---
In this  we will going to explain my code   of smart contract in solidity ...
---> 
straing with / SPDX-License-Identifier: MIT
pragma solidity 0.8.18; // 


Step 1. Firstlly  contract Intialization .. 
        Start contract MyToken .                             // DEclare the contract "myToken" .
          Declare public variable tokenName as "alexa"        and also define the public variable for token name like 'tokenName' ,
          Declare public variable  tokenAbbrv as " ale "      token abbreviation " tokenAbbrv" , and total supply " totalSupply" intializing them .//
          Declare public variable  totalSupply as "0 "      

Step 2. My contract is mapping for Balances...
        Declare  Mapping (address =>uint ) for  public balances  //Create a public mapping balances which maps an address to an unsigned integer. 
                                                                    This will store the token balance for each address. //
Step 3 .  Define a Mint Function ..
         Function mint( address, value )              // Define a function mint that takes two parameters an address and a value.
            Increase totalSupply by value                Increase the totalSupply by the given value.
            Increase  Balances [address] by value        Increase the balance of the given address by the same value. //
         end function 
                                                 
         
Step 4.  Define a burn Function ....
         Funtion burn( address ,value)                           // Define the burn function with take two parameters an address  and value 
          If balances [address] is greate than or equal to value   here for check the balance of the given address is greate than equal to the value or not .
             here decreases totalSupply by value                    if its true then dcreares the value of total supply value and also decrease the balance of the given address by the same value //
             decreases balances [address] by value 
          end if 
         also end function 
         
Step 5. End contract .
