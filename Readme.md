# 🗳️ VALOR – Verified Anonymous Ledger for Open Referendums  

**Secure. Anonymous. Scalable.**  
VALOR is a blockchain and cryptography-based online voting system designed to make elections **tamper-proof, transparent, and verifiable** without compromising voter privacy.  

---

## 📌 Overview  
Free and fair elections are the backbone of democracy, yet India’s voting systems face challenges of **tampering, duplicate voting, lack of transparency, and central trust dependency**.  

**VALOR** solves this by integrating:  
- **Blockchain immutability** for tamper-proof records  
- **Privacy-preserving cryptography** for anonymity  
- **Zero-Knowledge Proofs (ZKPs)** for verifiable correctness  
- **Homomorphic encryption** for tallying without decryption  

This creates a voting platform that is **secure, private, and scalable to millions of voters**.  

---

## 🛑 Problem Statement  
Current voting systems suffer from:  
- 🗂️ **Tampering Risks** – Ballots/EVMs can be manipulated.  
- 👤 **Fake or Duplicate Voting** – Weak identity verification.  
- 🔒 **Centralized Trust** – Dependence on one authority.  
- 🚫 **Lack of Transparency** – Voters can’t verify results.  
- ⚖️ **Scalability Issues** – Difficult to serve India’s massive electorate digitally.  

---

## 💡 The VALOR Solution  
VALOR ensures **“One Person, One Vote”** with full privacy.  

### 🔑 Core Features  
✔️ **Anonymous Voter Credentials** – No permanent personal data stored.  
✔️ **Secure OTP + EPIC/DOB Authentication** – Prevents fake/unauthorized logins.  
✔️ **Encrypted Ballots** – Votes encrypted locally with Paillier homomorphic encryption.  
✔️ **Zero-Knowledge Proofs** – Prove validity without exposing identity.  
✔️ **Immutable Blockchain Ledger** – Votes can’t be changed or deleted.  
✔️ **End-to-End Verifiability** – Voters can confirm their ballot is counted.  
✔️ **Bilingual UI (English + Hindi)** – Inclusivity for India’s diverse voters.  
✔️ **Scalable Architecture** – Designed for millions of users.  

---

## ⚙️ Workflow  

### 📝 Registration  
1. Enter **EPIC Number + DOB + Name + Phone Number**  
2. Verify via **OTP**  
3. System generates **anonymous digital credential**  

### 🔑 Login  
- Login with **EPIC + DOB/Password + OTP**  

### 🗳️ Voting  
- Select party/candidate  
- Vote **encrypted locally**  
- Submit to blockchain with **ZKP + nullifier**  
- Receive **confirmation message**  

### 📊 Results  
- Votes tallied using **homomorphic aggregation + threshold decryption**  
- Results published on **Blockscout blockchain explorer**  
- Public can audit tally, but individual votes remain secret  

---

## 🛠️ Tech Stack  

**Frontend** → React + TailwindCSS (multi-language support)  
**Backend** → Node.js + Express  
**Database** → Temporary encrypted storage (PostgreSQL/MongoDB)  
**Blockchain** → Ethereum Testnet / Polygon + Blockscout  
**Cryptography** →  
- Paillier Homomorphic Encryption  
- Zero-Knowledge Proofs (Circom + SnarkJS)  
- OTP verification system  

---

## 🚀 Roadmap  
- ✅ Prototype tested with **1,000–2,000 simulated voters** (IRIS 2026 demo)  
- 🔄 Optimize blockchain layer (scalability via rollups/sharding)  
- 🔐 Real-world integration with official EPIC verification  
- 🌍 Deployment on national-scale blockchain infra  

---

## 🎯 Impact  
VALOR demonstrates that **secure, transparent, and anonymous digital voting is achievable**.  
It combines **research-backed cryptography** with a **practical, user-friendly design** suited for India’s vast democracy.  

With VALOR, elections can finally be:  
- **Private** (votes remain secret)  
- **Verifiable** (anyone can audit results)  
- **Tamper-proof** (blockchain ensures immutability)  
- **Scalable** (from thousands → millions of voters)  

---

## 📚 References & Inspiration  
This project is built upon pioneering work in **electronic voting and cryptography**, including research by:  
- Josh Benaloh – End-to-End Verifiable Elections  
- Ben Adida – Helios Voting System  
- Edward Felten – Secure E-voting Systems  
- David Chaum – Mixnets & Voting Protocols  
- Antonio Russo, Hyunyeon Kim, Mohammed Awad, Gretchen A. Macht, Leonie S. Otte, Nicholas D. Bernardo – Blockchain & E-voting advancements  

Additionally, open-source tools like **paillier-bigint**, **Circom/snarkjs**, and blockchain documentation from **Ethereum/Polygon ecosystems** were critical in development.  

---

## 👨‍💻 Author  
Developed by **[Suyash Kumar]**, Grade **[11th Grade]**  
(Project submission for **IRIS National Science Fair 2026**)  

---
