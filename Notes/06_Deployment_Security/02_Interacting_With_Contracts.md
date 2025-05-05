# Talking to Deployed Contracts

---

### With JavaScript (ethers.js)

```js
const Hello = await ethers.getContractAt("Hello", "0x...address");
const greeting = await Hello.greet();
console.log(greeting);
```

---

### Changing a Value

```js
await Hello.setGreeting("Yo!");
```

---

### With Remix (Easier Way)

1. Paste contract code into Remix.
    
2. Compile it.
    
3. Use the “Deploy and Run” tab.
    
4. Paste contract address and ABI to interact with a deployed contract.
