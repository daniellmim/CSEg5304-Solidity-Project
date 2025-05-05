# Function Modifiers

- **Modifiers** add checks or logic to functions.
    

---

## Example Modifier

```solidity
modifier onlyOwner() {
    require(msg.sender == owner, "Not owner");
    _;
}
```

- `_;` means “run the main function here”.
    

---

## Using Modifiers

```solidity
function withdraw() public onlyOwner {
    // Only owner can run this
}
```

---

## Common Modifiers

- `onlyOwner`: Restricts access.
    
- `nonReentrant`: Prevents re-entry attack.
    
- `whenNotPaused`: Checks if contract is paused.