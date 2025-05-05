
# Reference Types in Solidity

These types store a reference (like a pointer), not the value directly.

---

## 1. **Array**

### Fixed-size:

```solidity
uint[3] numbers = [1, 2, 3];
```

### Dynamic:

```solidity
uint[] public list;

function add(uint x) public {
    list.push(x);
}
```

---

## 2. **Struct**

Custom type that groups variables.

```solidity
struct Person {
    string name;
    uint age;
}

Person public user = Person("Danny", 21);
```

---

## 3. **String & Bytes**

- `string` is for text.
    
- `bytes` is a dynamic byte array.
    

```solidity
string public name = "Danny";
bytes public data = "0x1234";
```
