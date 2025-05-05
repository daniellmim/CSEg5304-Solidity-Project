# Abstract Contracts

- Like interfaces, but can have some implemented functions.
    
- Can't be deployed directly.
    

---

## Example

```solidity
abstract contract Animal {
    function makeSound() public virtual view returns (string memory);
    function breathe() public pure returns (string memory) {
        return "Breathing";
    }
}

contract Dog is Animal {
    function makeSound() public pure override returns (string memory) {
        return "Bark";
    }
}
```
