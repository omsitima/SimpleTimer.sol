# SimpleTimer.sol
How to deploy a contract on Base Chain SimpleTimer.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract SimpleTimer {
    uint public startTime;

    constructor() {
        startTime = block.timestamp;
    }

    function getCurrentTime() public view returns (uint) {
        return block.timestamp;
    }
}
