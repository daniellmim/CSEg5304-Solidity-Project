 
# Events

- Let smart contracts **communicate with frontend** (e.g., React).
    
- Saved in transaction logs.
    

---

## Define an Event

```solidity
event Sent(address from, address to, uint amount);
```

---

## Emit an Event

```solidity
function send(address _to, uint _amount) public {
    emit Sent(msg.sender, _to, _amount);
}
```

---

## Use in Frontend

- You can **listen for events** using web3.js or ethers.js in a UI.
  