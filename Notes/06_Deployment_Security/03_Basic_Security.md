# Some Basic Security Tips

---

### 1. Use `require` to check stuff

```solidity
require(msg.sender == owner, "You can't do this");
```

---

### 2. Stop Reentrancy (Attack)

```solidity
bool locked;

modifier noReentry() {
    require(!locked, "Wait!");
    locked = true;
    _;
    locked = false;
}
```

---

### 3. Add Limits

Don’t let users send crazy values.

```solidity
require(amount < 100, "Too high!");
```

---

### 4. Use a `constructor` to set things once

```solidity
constructor() {
    owner = msg.sender;
}
```
