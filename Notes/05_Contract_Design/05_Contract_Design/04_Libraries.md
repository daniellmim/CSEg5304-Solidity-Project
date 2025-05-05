# Libraries

- Reusable code that doesn’t need to be a contract.
    
- Can be used without inheritance.
    

---

## Define a Library

```solidity
library Math {
    function add(uint a, uint b) internal pure returns (uint) {
        return a + b;
    }
}
```

---

## Use a Library

```solidity
using Math for uint;

contract Test {
    function addNumbers(uint x, uint y) public pure returns (uint) {
        return x.add(y);
    }
}
```
