# Inheritance in Solidity

- One contract can use code from another.
    
- Helps reuse and organize code.
    

---

## Basic Inheritance

```solidity
contract Parent {
    function sayHello() public pure returns (string memory) {
        return "Hello";
    }
}

contract Child is Parent {
    // Inherits sayHello()
}
```

---

## Overriding Functions

```solidity
contract Parent {
    function greet() public virtual pure returns (string memory) {
        return "Hi";
    }
}

contract Child is Parent {
    function greet() public override pure returns (string memory) {
        return "Hello from child";
    }
}
```
