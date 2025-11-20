---

# 🎓 Xperia – Decentralized Certificate Generation & Verification

## 🧠 Objective

To create a **secure**, **transparent**, and **tamper-proof** system for **generating** and **verifying** educational certificates using **blockchain technology** and **IPFS**.

---

## 📌 Introduction

**Xperia** uses **smart contracts** to ensure certificate authenticity and **IPFS** (via Pinata) for storing certificate files securely and accessibly.

---

## 🚀 Technologies Used

* **Blockchain**: Ethereum
* **Smart Contracts**: Solidity, Truffle
* **Local Blockchain Network**: Ganache
* **Decentralized Storage**: IPFS via Pinata
* **Front-End Interface**: Streamlit
* **Hosting**: Docker / Local installation

---

## 💡 Why This Project?

* Increasing cases of **certificate fraud**
* Inefficiencies in **manual verification processes**
* Growing demand for a **scalable** and **reliable** digital certificate system
* Need for **transparency** and **immutability** in academic records

---

## 🌐 Website Overview

The platform provides **two main interfaces**:

### 1. 🎓 Institute Interface

For certificate **generation** and **upload**

#### Steps:

1. **Login / Register**
2. **Generate PDF Certificate** (Streamlit)
3. **Upload to IPFS** (Pinata → Get CID)
4. **Interact with Smart Contract** (Store CID + Metadata on Blockchain)
5. **Receive Confirmation** (Transaction Hash + CID)

---

### 2. ✅ Verifier Interface

For **verifying** certificate authenticity

#### Steps:

1. **Access Verifier Page**
2. **Enter Certificate ID** or **Upload File**
3. **Query Blockchain** for CID & metadata
4. **Retrieve Certificate** from IPFS using CID
5. **Display Original Certificate** for validation

---

## ⚙️ Backend Workflow

### 🔸 Certificate Upload

* Institute logs in and generates a certificate
* Certificate is uploaded to Pinata (IPFS) → CID generated
* CID + metadata (e.g., student name, cert ID) sent to smart contract

### 🔸 Data Storage

* Smart contract stores CID + metadata **immutably** on the **Ethereum blockchain**

### 🔸 Certificate Verification

* Verifier queries blockchain with Certificate ID
* CID & metadata retrieved → used to fetch original file from IPFS
* Certificate is displayed for validation

---

## ✅ Features

* Tamper-proof and decentralized verification
* Fast & scalable certificate access
* Smart contract-driven automation
* Easy integration via Streamlit interface

---

## 🔮 Future Scope

* **Medical Sector**: Patient records, certification
* **Government**: Secure public records, e-voting
* **Corporate**: Employee credential verification

---

## ❓ FAQs

**Q1: What’s the purpose of this project?**
To create a secure and verifiable blockchain-based certificate system for institutions.

**Q2: How does blockchain ensure security?**
By storing data in an immutable, decentralized ledger—making tampering virtually impossible.

**Q3: What is IPFS and why use it?**
IPFS is a decentralized storage system used to host and retrieve digital certificate files reliably.

**Q4: How do verifiers check a certificate?**
By entering the certificate ID on the platform, which fetches the record from blockchain and displays it via IPFS.

**Q5: What’s the role of smart contracts?**
They handle secure storage and retrieval of certificate data, enforcing trust and automation.

**Q6: How is this better than traditional methods?**
It eliminates fraud, cuts down verification time, and ensures data integrity.

---

## 👨‍💻 Team

**Team Xperia** – Presented at **Industry Conclave 2024 – Project Expo**

---