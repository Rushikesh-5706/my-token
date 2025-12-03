# 📘 Learning Reflection — ERC-20 Token Project (MyToken)

This project was my first hands-on experience with building a cryptocurrency token on Ethereum.  
By implementing the ERC-20 standard myself, I gained a deeper understanding of how tokens work behind the scenes and how decentralized assets are structured.

---

## 🔹 What I Learned

### **1. The Structure of ERC-20 Tokens**
I learned how ERC-20 tokens follow a strict interface that includes:
- balance tracking  
- token transfers  
- approvals and delegated transfers  
- event emissions  

This ensures compatibility across wallets, exchanges, and smart contracts.

### **2. Importance of Decimals**
Understanding decimals (usually 18) helped me realize how token amounts are represented in smallest units, similar to how ETH uses wei.

### **3. Using Mappings for Balances & Allowances**
Mappings allowed me to maintain:
- `balanceOf[address]`  
- `allowance[owner][spender]`

This taught me about efficient storage and lookups on the Ethereum Virtual Machine (EVM).

### **4. The Difference Between transfer and transferFrom**
- **transfer** lets the sender send tokens directly.  
- **transferFrom** allows a third party (spender) to move tokens after being approved.

This is crucial for DApps like exchanges and marketplaces.

### **5. Event Logging**
The ERC-20 standard requires `Transfer` and `Approval` events.  
I learned why logs are essential:
- They allow block explorers to index token activity  
- They help users track movements transparently  
- They provide an audit trail for external systems  

### **6. Defensive Coding**
I implemented checks such as:
- Preventing transfers to the zero address  
- Ensuring sufficient balance before transfers  
- Ensuring allowance is adequate before delegated transfers  

This taught me the importance of security even in simple contracts.

### **7. Using Remix for Smart Contract Development**
I learned how to:
- Create and compile Solidity files  
- Deploy contracts to a virtual blockchain (Remix VM)  
- Test calls and transactions  
- Inspect logs and events  
- Debug errors like insufficient balance or allowance  

### **8. End-to-End Token Workflow**
I performed:
- Compilation  
- Deployment  
- Balance checks  
- Token transfers  
- Setting allowances  
- Delegated transfers  

This gave me confidence in developing and interacting with real smart contracts.

---

## 🔹 Challenges I Faced

- Understanding how allowances decrease after transferFrom  
- Remembering to switch accounts for different roles (owner, spender, recipient)  
- Working with large integer values using 18 decimals  
- Ensuring correct addresses were used when calling functions  

Each challenge helped me build stronger debugging skills.

---

## 🔹 Final Thoughts

This ERC-20 project provided a strong foundation in Solidity programming and token mechanics.  
I now feel confident creating, deploying, and testing smart contracts on Ethereum.

It also helped me understand why ERC-20 remains the most widely used token standard in the crypto ecosystem.
