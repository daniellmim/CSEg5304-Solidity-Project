# Setting Up Solidity

## 1. Install Node.js & npm

You need Node.js and npm for most tools.

```bash
sudo apt install nodejs
sudo apt install npm
```

---

## 2. Install Hardhat (Solidity dev tool)

```bash
npm install --save-dev hardhat
npx hardhat
```

Choose: “Create a basic sample project”

---

## 3. Project Structure

```text
myproject/
├── contracts/         // Solidity files (.sol)
├── scripts/           // Deployment scripts
├── test/              // Test files
├── hardhat.config.js  // Config file
```

---

## 4. Create a Contract

Inside `contracts/Hello.sol`:

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract Hello {
    string public greet = "Hi!";
}
```

---

## 5. Compile

```bash
npx hardhat compile
```