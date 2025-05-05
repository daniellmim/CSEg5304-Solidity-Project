
# Solidity Basic Syntax

---

## Version Declaration

Always add this on top:

```solidity
pragma solidity ^0.8.0;
```

---

## Contract

```solidity
contract MyContract {
    // Code goes here
}
```

---

## Variables

```solidity
uint public myNumber = 10;
string public myText = "Hello";
bool public isActive = true;
```

---

## Functions

```solidity
function getNumber() public view returns (uint) {
    return myNumber;
}
```

---

## Constructor

Runs once when contract is deployed:

```solidity
constructor() {
    myNumber = 100;
}
```

---

## Comments

```solidity
// Single line

/*
Multi-line
comment
*/
```
