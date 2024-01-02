# RedBelly </br>

## **Token Contract Documentation** </br>

**Contract Address:** `0xc2211ccba9a63f815e1200c302488e6af2b76750` </br>

**Token Name :** `Redbelly Devnet`  </br>

**Token Symbol :**  `BU` </br>

 [Remix IDE](https://remix.ethereum.org/). Remix is one of the commonly used development environments for smart contracts on Ethereum.

[Open Remix](https://remix.ethereum.org/) and click on the `New File`

Name your file, in our case we've named it `Redbelly.sol` - yes, that [famous token standard](https://eips.ethereum.org/EIPS/eip-20)


Now add code. 

pragma solidity 0.8.17;

 // SPDX-License-Identifier: MIT

 contract Bustaaal { string public name = "Redbelly Devnet"; string public symbol = "BU"; uint8 public decimals = 18; uint256 public totalSupply = 100000000;

 mapping (address => uint256) public balances; address public owner;

 constructor() { owner = msg.sender; balances[owner] = totalSupply; }

 function transfer(address recipient, uint256 amount) public { require(balances[msg.sender] >= amount, "Insufficient balance."); balances[msg.sender] -= amount; balances[recipient] += amount; } }


On the left sidebar, you will click on Solidity compiler and Compile erc20.sol

```text
Solidity Compiler >>> Compile Contract
```

Now click to the `Deploy & Run Transactions` on the left in the sidebar and open Metamask to check if is our account connected. If it's connected you can skip to next steps


You will see your contract has been successfully deployed.

#### Reach us for more engagement <a id="reach-us-for-more-engagement"></a>
