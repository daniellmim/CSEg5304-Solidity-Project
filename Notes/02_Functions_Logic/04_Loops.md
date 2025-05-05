# Loops in Solidity

---

## For Loop

```solidity
for (uint i = 0; i < 10; i++) {
    // repeat this 10 times
}
```

---

## While Loop

```solidity
uint i = 0;
while (i < 5) {
    i++;
}
```

---

## Avoid Infinite Loops

- Gas is limited. Don’t use unbounded loops!