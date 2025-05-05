# Function & Variable Visibility

Controls who can access functions or variables.

---

## 1. **public**

- Can be called from anywhere.
    

```solidity
uint public count;

function getCount() public view returns (uint) {
    return count;
}
```

---

## 2. **private**

- Only inside the same contract.
    

```solidity
uint private secret;

function setSecret(uint _x) private {
    secret = _x;
}
```

---

## 3. **internal**

- Only inside this contract and children (inherited contracts).
    

```solidity
uint internal value;
```

---

## 4. **external**

- Only callable from outside the contract.
    

```solidity
function externalFunc() external {
    // can't call this inside the contract
}
```
