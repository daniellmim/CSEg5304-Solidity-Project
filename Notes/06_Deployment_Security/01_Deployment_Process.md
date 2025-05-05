# How to Deploy a Smart Contract

I used **Hardhat** to deploy a contract. Here’s how I did it step by step:

---

### 1. Make Your Contract

```solidity
// contracts/Hello.sol
pragma solidity ^0.8.0;

contract Hello {
    string public greet = "Hi!";
}
```

---

### 2. Write a Deploy Script

```js
// scripts/deploy.js
async function main() {
    const Hello = await ethers.getContractFactory("Hello");
    const hello = await Hello.deploy();
    await hello.deployed();
    console.log("Contract deployed to:", hello.address);
}
main();
```

---

### 3. Compile the Contract

```bash
npx hardhat compile
```

---

### 4. Run it on Local Network

```bash
npx hardhat run scripts/deploy.js --network localhost
```

---

### 5. (Optional) Deploy to a Testnet

If I wanted to put it on a real test network, I’d add network info in `hardhat.config.js` and use my wallet + Infura or Alchemy.
