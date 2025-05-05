# State Variables

- Stored on the blockchain.
    
- Keep data between function calls.
    

---

## Declare

```solidity
string public name = "Danny";
uint public count = 0;
```

---

## Access & Change

```solidity
function updateCount() public {
    count += 1;
}
```

---

## Types

- You can use any type: `uint`, `bool`, `address`, `mapping`, `struct`, etc.
    

---

## Storage Cost

- State variables cost **gas**.
    
- Use them wisely!
   