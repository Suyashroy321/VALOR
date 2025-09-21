# VALOR - Verified Autonomous Ledger for Online Referendums

## Project Overview 📌

VALOR is a blockchain and cryptography-based online voting system designed to make elections secure, private, transparent, and scalable. It directly addresses challenges faced in current voting systems in India and worldwide — such as duplicate voting, tampering, lack of transparency, and dependence on centralized authorities.

The project leverages blockchain immutability, privacy-preserving cryptography, homomorphic encryption, and zero-knowledge proofs (ZKPs) to create a verifiable yet anonymous digital democracy platform.

## The Problem 🛑

Traditional voting systems — whether paper-based or EVMs — suffer from:

* **Tampering Risks** - Ballots/EVMs can be manipulated
* **Lack of Transparency** - Voters can't verify results independently
* **Duplicate / Fake Voting** - Weak identity verification allows abuse
* **Centralized Trust** - Current systems rely on one authority to be 100% honest
* **Scalability & Accessibility** - Difficult to serve India's 900+ million voters in a transparent digital system

## The Solution: VALOR 💡

VALOR ensures "One Person, One Vote" without compromising voter privacy.

### Core Features 🔑

#### Anonymous Voter Credentials
- Voter registers using EPIC (Voter ID) + Date of Birth + Phone verification
- Details are encrypted and never stored permanently
- A unique anonymous credential is generated for each voter

#### Secure Authentication
- **Registration:** EPIC + DOB + Phone OTP + Password creation
- **Login:** Voter ID + DOB/Password + OTP
- Ensures only legitimate voters can access the ballot

#### Vote Casting
- Each ballot is encrypted locally on the voter's device (Paillier homomorphic encryption)
- Voter confirms choice → encrypted vote submitted
- Duplicate voting prevented using cryptographic nullifiers

#### Blockchain Ledger
- Encrypted ballots + proofs stored immutably on blockchain
- No one can alter or delete votes
- Public can audit results without seeing individual votes

#### Zero-Knowledge Proofs (ZKPs)
- Guarantee that each vote is valid
- Ensures privacy + verifiability without revealing identities

#### End-to-End Verifiability
- Voters can check that their ballot is included in the final tally
- Results are publicly auditable via a blockchain explorer (Blockscout)

#### Bilingual & Scalable
- Interface supports Hindi + English for inclusivity
- Architecture scales from 1,000 test users → millions of voters

## How VALOR Works ⚙️

### Registration
1. Voter enters EPIC number, DOB, and phone number
2. OTP is sent → after verification, voter sets password
3. System generates an anonymous credential (cryptographic key)

### Login
1. Voter logs in using EPIC + DOB/Password + OTP
2. Gains access to election dashboard

### Voting
1. Voter selects candidate/party
2. Vote encrypted locally → submitted to blockchain with ZKP
3. Voter sees confirmation ("Your vote has been cast successfully")

### Result Day
1. Encrypted votes tallied using homomorphic aggregation + threshold decryption
2. Blockchain explorer link provided for full transparency
3. Everyone can verify tally, no one can trace individual votes

## Tech Stack 🛠️

- **Frontend:** React + TailwindCSS (Bilingual UI: English/Hindi)
- **Backend:** Node.js / Express
- **Database:** Encrypted temporary storage (PostgreSQL / MongoDB)
- **Blockchain:** Ethereum testnet / Polygon (with Blockscout for audit)
- **Cryptography:**
  - Homomorphic Encryption (Paillier)
  - Zero-Knowledge Proofs (Circom / SnarkJS)
  - OTP-based verification (Twilio or mock OTP system for demo)

## Roadmap 🚀

- ✅ Prototype with 1,000–2,000 simulated voters (IRIS National Science Fair)
- ⚙️ Optimization for scalability (sharding, rollups for blockchain efficiency)
- 🔐 Integration of multi-factor identity checks
- 🌍 Deployment on scalable blockchain infrastructure for national use

## Impact 🎯

VALOR proves that secure, anonymous, and transparent digital voting is possible. It introduces innovations like ZKP-based verifiability, blockchain immutability, and bilingual accessibility — making it uniquely suited for India's scale of democracy.

This project can pave the way for future electoral reforms, ensuring elections are tamper-proof, transparent, and accessible to all citizens.