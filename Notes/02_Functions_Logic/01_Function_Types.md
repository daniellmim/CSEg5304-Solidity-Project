# Types of Functions in Solidity

---

## 1. **View Function**

- Reads data, doesn't change it.
    

```solidity
function get() public view returns (uint) {
    return myNumber;
}
```

---

## 2. **Pure Function**

- Doesn’t read or write to storage.
    

```solidity
function add(uint a, uint b) public pure returns (uint) {
    return a + b;
}
```

---

## 3. **Payable Function**

- Can receive Ether.
    

```solidity
function deposit() public payable {
    // Ether received
}
```

---

## 4. **Internal Function**

- Can only be called inside this contract or by contracts that inherit it.
    

```solidity
function internalFunc() internal {
    // internal logic
}
```

---

## 5. **External Function**

- Can be called from outside the contract.
    

```solidity
function externalFunc() external {
    // accessible externally
}
```

---

## 6. **Private Function**

- Only used inside the same contract.
    

```solidity
function privateFunc() private {
    // not visible anywhere else
}
```