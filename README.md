# Project Title

Simple overview of use/purpose.

## Description

An in-depth paragraph about your project and overview of use.

## Getting Started

### Installing

* How/where to download your program
* Any modifications needed to be made to files/folders

### Executing program

* How to run the program
* Step-by-step bullets
```
code blocks for commands
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract Alber {
    uint256 public myNumber;

    function setNumber(uint256 _num) external {
        // Using require() to validate input
        require(_num != 0, "Number cannot be zero");
        
        // Using assert() to validate internal state
        assert(myNumber + _num > myNumber);

        // Using revert() to revert the transaction
        if (_num > 100) {
            revert("Number is too large");
        }

        myNumber = _num;
    }
}
```

## Help

Any advise for common problems or issues.
```
command to run if program contains helper info
```

## Authors

Contributors names and contact info

ex. Alber C Aquino  
ex. https://www.facebook.com/DBGTK


## License

This project is licensed under the [SPDX-MIT] License - see the LICENSE.md file for details
