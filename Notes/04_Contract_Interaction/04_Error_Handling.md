# Error Handling

Make sure your contract behaves safely when things go wrong.

---

## require()

Checks conditions before running.

```solidity
require(msg.sender == owner, "Not the owner");
```

---

## revert()

Manual error.

```solidity
if (x < 1) {
    revert("x is too small");
}
```

---

## assert()

Used to check for bugs or internal errors.

```solidity
assert(balance >= 0);
```

---

## Custom Errors (Gas Efficient)

```solidity
error NotOwner();

function onlyOwner() public {
    if (msg.sender != owner) {
        revert NotOwner();
    }
}
```