# Control Flow Statements

---

## if / else

```solidity
if (x > 10) {
    // do something
} else {
    // do something else
}
```

---

## require

Stops execution if false.

```solidity
require(x > 0, "x must be > 0");
```

---

## revert

Manually throw an error.

```solidity
if (x < 5) {
    revert("Too small");
}
```

---

## assert

Used for internal errors and invariants.

```solidity
assert(balance >= 0);
```