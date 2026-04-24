<div align="center">
  <img src="assets/JeffreyWooTimeBank.png" alt="JeffreyWooTimeBankBanner" width="1200" height="800" />
</div>

## 📊 Overview
         
> **Not your typical community exchange app!**

**JeffreyWoo TimeBank** is a decentralized, AI-powered timebanking DApp that enables communities to exchange skills, services, and care using time credits as currency. Built on a blockchain-inspired, hash-chained ledger, every transaction is cryptographically linked, tamper-resistant, and publicly verifiable — ensuring trust without intermediaries.  

AI-driven matching intelligently connects neighbors by skills and needs, fostering collaboration across generations and professions. The principle is simple yet powerful: **1 hour given = 1 hour earned**. By combining transparent ledger technology with adaptive AI, it transforms volunteering into a sustainable, equitable ecosystem where time itself becomes the foundation of community value.

## ⏰ Timebanking System

<img src="assets/JeffreyWooTimeBank16.png" alt="JeffreyWooTimeBank16" width="1200" height="800" />

**JeffreyWoo TimeBank** is built on the principle that everyone’s time has equal value. It transforms community service into a transparent, trust‑based exchange system where time itself becomes the currency.

### 💡 Core Concept

- Timebanking allows members to earn time credits by providing services and spend/donate those time credits to receive help or support others.
- The guiding rule is simple: **1 hour given = 1 hour earned**.

### 🔄 How It Works

#### 1. Service Exchange  
Members offer skills — tutoring, caregiving, design review, repairs, etc. — and record the time spent helping others.

#### 2. Earning Time Credits  
Each hour of service generates a one-time credit stored securely in the ledger.

#### 3. Spending/Donating Time Credits  
Members use earned credits to request services from others, or donate them to community pools/charities/individuals in need, creating a continuous cycle of giving and receiving, and promoting generosity and social inclusion.

#### 4. Flexible Reciprocity  
Exchanges don’t need to be one‑to‑one. Members can give help to one person and receive help from another, fostering community collaboration or a continuous cycle of goodwill.

#### 5. Transparent Ledger  
Every “earn”, “spend/donate" transaction is recorded in the hash‑chained ledger, ensuring integrity and public verifiability.

### 🔗 Blockchain‑Inspired Transparency

- Each transaction is cryptographically linked to the previous one using **prevHash** and **entryHash**.
- The ledger forms an immutable chain of service records, preventing tampering and ensuring accountability.
- This blockchain‑inspired design provides **trust without intermediaries**, making time exchanges secure, auditable, and community-driven.

## ✨ What It Does

🤝 **Community Time Exchange** — trade time and skills directly with others through smart contracts  
🧠 **AI Matching Engine** — intelligently connects users based on skill profiles, availability, and community needs  
🔗 **Blockchain Transparency** — ensures secure, immutable records of time transactions  
🌍 **Global & Local Integration** — supports Hong Kong community exchanges while connecting to global timebank networks  
🔒 **Digital Identity & Trust Layer** — verifies participants via decentralized identity (DID) and reputation scoring

## 🤝 Social Impact

This project demonstrates how technology can reshape community collaboration by:  
- Empowering individuals to value time and care equally, regardless of profession or income
- Building trust and social connection across neighborhoods through transparent, decentralized time exchange
- Encouraging volunteering, mutual aid, social inclusion, and intergenerational cooperation
- Promoting sustainable community development through equitable resource sharing
- Integrating AI to optimize skill matching and time utilization
- Enables members to donate time to support vulnerable groups.

## 🚀 Why Choose JeffreyWoo TimeBank

Most apps focus on money. **JeffreyWoo TimeBank** focuses on time — the most universal currency.
It merges AI intelligence with blockchain fairness, creating a new way to exchange value that’s human-centered, transparent, and future-ready.

## 🧩 Core Concepts

|Concept	| Description|
|---------|------------|
|**Time as Currency**	| Every hour of service equals one hour of credit, regardless of skill type|
|**Smart Contracts**	| Automate time transactions securely on the blockchain|
|**AI Skill Matching**	| Suggests optimal exchanges based on user profiles and community demand|
|**Decentralized Identity (DID)**	| Builds trust through verifiable digital identities|
|**Community Analytics**	| Tracks engagement, contribution, and social impact metrics|

## 🏗️ System Architecture Overview — Current State
<pre lang="markdown">
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                              PRESENTATION LAYER                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                         User Interface (React)                                │  │
│  │                           TypeScript Frontend                                 │  │
│  │                      (Tailwind CSS / Framer Motion)                           │  │
│  │                                                                               │  │
│  │  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────────────────┐    │  │
│  │  │  Service Browse │  │  Ledger Viewer  │  │  Profile & Dashboard        │    │  │
│  │  │  & Request      │  │  (Live Updates) │  │  (Credits Balance)          │    │  │
│  │  └─────────────────┘  └─────────────────┘  └─────────────────────────────┘    │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────────────────────────────┘
                                              │
                                              ▼
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                               APPLICATION LAYER                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                         Frontend Logic Layer                                  │  │
│  │                    (State Management / API Calls)                             │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
│                                              │                                      │
│              ┌───────────────────────────────┼───────────────────────────────┐      │
│              ▼                               ▼                               ▼      │
│  ┌───────────────────────┐   ┌───────────────────────────┐   ┌─────────────────────┐│
│  │   AI Matching Engine  │   │    Backend & API Layer    │   │  User & Identity    ││
│  │                       │   │     (Node.js / FastAPI)   │   │     Management      ││
│  │ ┌───────────────────┐ │   │                           │   │                     ││
│  │ │ Gemini API /      │ │   │  ┌─────────────────────┐  │   │ ┌─────────────────┐ ││
│  │ │ GPT-4o-ca         │ │   │  │ REST / GraphQL API  │  │   │ │ Basic User Auth │ ││
│  │ └───────────────────┘ │   │  └─────────────────────┘  │   │ │ (Email/Password)│ ││
│  │                       │   │                           │   │ └─────────────────┘ ││
│  │ ┌───────────────────┐ │   │  ┌─────────────────────┐  │   │ ┌─────────────────┐ ││
│  │ │ Skill-Based       │ │   │  │ WebSocket Gateway   │  │   │ │ Profile Storage │ ││
│  │ │ Matching          │ │   │  │ (Real-time ledger   │  │   │ │ (PostgreSQL)    │ ││
│  │ └───────────────────┘ │   │  │  updates)           │  │   │ └─────────────────┘ ││
│  └───────────────────────┘   │  └─────────────────────┘  │   └─────────────────────┘│
│                              └───────────────────────────┘                          │
└─────────────────────────────────────────────────────────────────────────────────────┘
                                              │
                                              ▼
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                              DATA & STORAGE LAYER                                   │
│                                                                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                         Off-Chain Storage                                     │  │
│  │                                                                               │  │
│  │  ┌─────────────────────────┐         ┌─────────────────────────────────────┐  │  │
│  │  │       PostgreSQL        │         │              Redis                  │  │  │
│  │  │                         │         │                                     │  │  │
│  │  │  ┌─────────────────────┐│         │  ┌───────────────────────────────┐  │  │  │
│  │  │  │  User Profiles      ││         │  │  Session Cache                │  │  │  │
│  │  │  │  • Basic info       ││         │  └───────────────────────────────┘  │  │  │
│  │  │  │  • Skills offered   ││         │                                     │  │  │
│  │  │  │  • Reputation       ││         │  ┌───────────────────────────────┐  │  │  │
│  │  │  └─────────────────────┘│         │  │  Real-time Ledger Cache       │  │  │  │
│  │  │                         │         │  └───────────────────────────────┘  │  │  │
│  │  │  ┌─────────────────────┐│         └─────────────────────────────────────┘  │  │
│  │  │  │  Service Listings   ││                                                  │  │
│  │  │  │  • Title/Desc       ││                                                  │  │
│  │  │  │  • Duration         ││                                                  │  │
│  │  │  │  • Provider         ││                                                  │  │
│  │  │  └─────────────────────┘│                                                  │  │
│  │  └─────────────────────────┘                                                  │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
│                                              │                                      │
│                                              ▼                                      │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                    TRANSACTION LEDGER TABLES (Core Feature)                   │  │
│  │                                                                               │  │
│  │  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────────────┐   │  │
│  │  │    EARN     │  │    SPEND    │  │   DONATE    │  │    POOL PAYOUT      │   │  │
│  │  │   Table     │  │   Table     │  │   Table     │  │      Table          │   │  │
│  │  ├─────────────┤  ├─────────────┤  ├─────────────┤  ├─────────────────────┤   │  │
│  │  │ • id        │  │ • id        │  │ • id        │  │ • id                │   │  │
│  │  │ • user_id   │  │ • from_id   │  │ • from_id   │  │ • pool_id           │   │  │
│  │  │ • minutes   │  │ • to_id     │  │ • to_id     │  │ • recipient_id      │   │  │
│  │  │ • timestamp │  │ • minutes   │  │ • minutes   │  │ • minutes           │   │  │
│  │  │ • service   │  │ • timestamp │  │ • timestamp │  │ • timestamp         │   │  │
│  │  │   id        │  │ • service   │  │ • pool_id   │  │ • reason            │   │  │
│  │  │ • memo      │  │   id        │  │ • memo      │  │ • approved_by       │   │  │
│  │  └─────────────┘  │ • memo      │  └─────────────┘  └─────────────────────┘   │  │
│  │                   └─────────────┘                                             │  │
│  │                                                                               │  │
│  │  ┌─────────────────────────────────────────────────────────────────────────┐  │  │
│  │  │              Hash-Chained Linkage (Cryptographic Integrity)             │  │  │
│  │  │                                                                         │  │  │
│  │  │   Each transaction stores:                                              │  │  │
│  │  │   • prevHash  → Hash of the previous transaction's entryHash            │  │  │
│  │  │   • entryHash → SHA-256(concatenated transaction fields + prevHash)     │  │  │
│  │  │                                                                         │  │  │
│  │  │   [Record 1] ──hash──→ [Record 2] ──hash──→ [Record 3] ──hash──→ ...    │  │  │
│  │  │   (prevHash=0)         (prevHash=H1)        (prevHash=H2)               │  │  │
│  │  └─────────────────────────────────────────────────────────────────────────┘  │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────────────────────────────┘
                                              │
                                              ▼
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                           BLOCKCHAIN-INSPIRED LAYER                                 │
│                                                                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                    Hash-Chained Ledger Implementation                         │  │
│  │                              (Current)                                        │  │
│  │                                                                               │  │
│  │  ┌─────────────────────────────────────────────────────────────────────────┐  │  │
│  │  │                      Cryptographic Verification                         │  │  │
│  │  │                                                                         │  │  │
│  │  │   • Tamper-evident chain                                                │  │  │
│  │  │   • Public verifiability                                                │  │  │
│  │  │   • No external blockchain required                                     │  │  │
│  │  │   • Trust without intermediaries                                        │  │  │
│  │  └─────────────────────────────────────────────────────────────────────────┘  │  │
│  │                                                                               │  │
│  │  ┌─────────────────────────────────────────────────────────────────────────┐  │  │
│  │  │                    1 Hour Given = 1 Hour Earned                         │  │  │
│  │  │                         (Time Credit Rule)                              │  │  │
│  │  └─────────────────────────────────────────────────────────────────────────┘  │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────────────────────────────┘
                                              │
                                              ▼
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                              ANALYTICS & INSIGHTS LAYER                             │
│                                                                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                         Community Analytics Platform                          │  │
│  │                                                                               │  │
│  │  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────────────────────┐│  │
│  │  │  Live Ledger    │  │  User Activity  │  │  Community Impact               ││  │
│  │  │  Viewer         │  │  Dashboard      │  │  • Total hours exchanged        ││  │
│  │  │  • All Txns     │  │  • Credits      │  │  • Active members               ││  │
│  │  │  • Hash chain   │  │    balance      │  │  • Services offered             ││  │
│  │  │  • Public log   │  │  • Tx history   │  │  • Pool donations               ││  │
│  │  └─────────────────┘  └─────────────────┘  └─────────────────────────────────┘│  │
│  │                                                                               │  │
│  │  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────────────────────┐│  │
│  │  │  AI-Powered     │  │  Skill Demand   │  │  Personalized                   ││  │
│  │  │  Recommendations│  │  Analytics      │  │  Matching Suggestions           ││  │
│  │  │  • Next actions │  │  • Popular      │  │  • Based on skills              ││  │
│  │  │  • Skill match  │  │    services     │  │  • Based on history             ││  │
│  │  └─────────────────┘  └─────────────────┘  └─────────────────────────────────┘│  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────────────────────────────┘</pre>

## 🤖 Tech Stack

- **Language:** TypeScript, HTML
- **Framework:** React (Next.js optional)
- **Backend:** Node.js + FastAPI (for AI integration)
- **Blockchain:** Ethereum / Polygon (Smart Contracts via Solidity)
- **AI Models:** Gemini API, ChatAnywhere GPT 4o ca
- **Database:** PostgreSQL, Redis
- **UI:** Tailwind CSS + Recharts + Framer Motion

## 🧠 AI Techniques Applied

Artificial Intelligence is integrated into **JeffreyWoo TimeBank** to make time exchanges smarter, fairer, and more efficient. While the ledger ensures transparency and trust, AI adds intelligence to the way communities connect and collaborate.

|Key Application|Description|
|----------------|-----------|
|**Skill & Need Matching**|AI analyzes participant profiles, skills, and availability to recommend optimal exchanges — ensuring that time credits flow where they are most valuable.|
|**Community Insights**|Machine learning models detect patterns in service demand and supply, helping communities anticipate needs (e.g., tutoring spikes before exams, caregiving demand during holidays).|
|**Personalized Recommendations**|AI suggests opportunities for participants based on their past contributions, reputation, and preferences — encouraging ongoing engagement.|
|**Trust & Reputation Scoring**|AI evaluates contribution history and feedback to generate reputation scores, strengthening accountability and reducing the risk of misuse.|
|**Scalability Across Communities**|AI enables interoperability between local timebanks, predicting cross‑community exchanges and fostering global collaboration.|

## 🔗 Blockchain & Ledger Techniques Applied

**JeffreyWoo TimeBank** leverages a hash‑chained ledger architecture inspired by blockchain principles to ensure trust, transparency, and accountability in time credit exchanges.

|Core Feature|Description|
|-------------|-----------|
|**Hash‑Chained Transactions**|Every service exchange is recorded as a transaction linked cryptographically to the previous one, forming an immutable chain of records.|
|**Public Verifiability**|Transactions are auditable and tamper‑resistant, ensuring community trust without requiring centralized intermediaries.|
|**Time Credits as Currency**|Each hour of service provided equals one hour earned. Credits circulate freely, enabling flexible exchanges across the community.|
|**AI‑Enhanced Matching**|AI algorithms connect participants by skills and needs, ensuring efficient and equitable distribution of time credits.|
|**Decentralized Identity & Reputation**|Each participant maintains a verifiable digital identity, with reputation scores built from contribution history.|

## ⚙️ Formation of the Hash‑Chained Ledger

**JeffreyWoo TimeBank** does not rely on a public blockchain like **Ethereum or Polygon** by default. Instead, it implements a **blockchain‑inspired hash‑chained ledger** inside its database to ensure immutability and verifiability of time credit transactions.

### How It Works

**1. Transaction Entry**  

Each service exchange (e.g., tutoring, bike repair) is recorded as a row in the ledger with all relevant fields: Sender, Recipient, Minutes, Memo, Timestamp, etc.

**2. PrevHash**

- The **prevHash** field stores the hash of the previous transaction’s **entryHash**.
- This links each new record to the one before it, forming a continuous chain.

**3. EntryHash**

- The **entryHash** is computed by concatenating the transaction’s fields, including ID, Index, Kind (Grant, Exchange, Donation, Pool Payout), From ID, From Name, To ID, To Name, Minutes, Memo, Related Service ID, Related Service Title, Created At, and **prevHash**.
- This concatenated string is then hashed using a cryptographic function such as **SHA‑256**.

**4. Chain Integrity**

- Because each transaction depends on the hash of the previous one, altering any record breaks the chain.
- This makes the ledger tamper‑evident, similar to how blocks are linked in a blockchain.

## 🪙 System Architecture Overview — Future State (with Roadmap Integration)
<pre lang="markdown">
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                              PRESENTATION LAYER                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                         User Interface (React)                                │  │
│  │                           TypeScript Frontend                                 │  │
│  │                      (Tailwind CSS / Framer Motion)                           │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────────────────────────────┘
                                              │
                                              ▼
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                               APPLICATION LAYER                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                         Frontend Logic Layer                                  │  │
│  │                    (State Management / API Calls)                             │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
│                                              │                                      │
│              ┌───────────────────────────────┼───────────────────────────────┐      │
│              ▼                               ▼                               ▼      │
│  ┌───────────────────────┐   ┌───────────────────────────┐   ┌─────────────────────┐│
│  │   AI Matching Engine  │   │    Backend & API Layer    │   │  Decentralized      ││
│  │                       │   │     (Node.js / FastAPI)   │   │  Identity (DID)     ││
│  │ ┌───────────────────┐ │   │                           │   │                     ││
│  │ │ Gemini API /      │ │   │  ┌─────────────────────┐  │   │ ┌─────────────────┐ ││
│  │ │ GPT-4o-ca         │ │   │  │ REST / GraphQL API  │  │   │ │ Verifiable      │ ││
│  │ └───────────────────┘ │   │  └─────────────────────┘  │   │ │ Digital IDs     │ ││
│  │ ┌───────────────────┐ │   │                           │   │ └─────────────────┘ ││
│  │ │ Demand/Supply     │ │   │  ┌─────────────────────┐  │   │ ┌─────────────────┐ ││
│  │ │ Prediction        │ │   │  │ WebSocket Gateway   │  │   │ │ Reputation      │ ││
│  │ │ (Real-time)       │ │   │  │ (Real-time updates) │  │   │ │ Scoring Engine  │ ││
│  │ └───────────────────┘ │   │  └─────────────────────┘  │   │ └─────────────────┘ ││
│  └───────────────────────┘   └───────────────────────────┘   └─────────────────────┘│
└─────────────────────────────────────────────────────────────────────────────────────┘
                                              │
                                              ▼
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                              DATA & STORAGE LAYER                                   │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                    Off-Chain Storage (Current + Caching)                      │  │
│  │  ┌─────────────────────────┐         ┌─────────────────────────────────────┐  │  │
│  │  │     PostgreSQL          │         │              Redis                  │  │  │
│  │  │  • User Profiles        │         │  • Session Management               │  │  │
│  │  │  • AI Match Cache       │         │  • Real-time Analytics Cache        │  │  │
│  │  │  • Analytics Data       │         │  • Rate Limiting                    │  │  │
│  │  └─────────────────────────┘         └─────────────────────────────────────┘  │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
│                                              │                                      │
│                                              ▼                                      │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                    TRANSACTION LEDGER TABLES (Logical Model)                  │  │
│  │                                                                               │  │
│  │  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────────────┐   │  │
│  │  │    EARN     │  │    SPEND    │  │   DONATE    │  │    POOL PAYOUT      │   │  │
│  │  │  Table      │  │   Table     │  │   Table     │  │      Table          │   │  │
│  │  ├─────────────┤  ├─────────────┤  ├─────────────┤  ├─────────────────────┤   │  │
│  │  │ • user_id   │  │ • from_id   │  │ • from_id   │  │ • pool_id           │   │  │
│  │  │ • minutes   │  │ • to_id     │  │ • to_id     │  │ • recipient_id      │   │  │
│  │  │ • timestamp │  │ • minutes   │  │ • minutes   │  │ • minutes           │   │  │
│  │  │ • service   │  │ • timestamp │  │ • timestamp │  │ • timestamp         │   │  │
│  │  │   details   │  │ • service   │  │ • pool_id   │  │ • approval_hash     │   │  │
│  │  └─────────────┘  └─────────────┘  └─────────────┘  └─────────────────────┘   │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────────────────────────────┘
                                              │
                                              ▼
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                            BLOCKCHAIN / SMART CONTRACT LAYER                        │
│                                    (Future)                                         │
│                                                                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                         SOLIDITY SMART CONTRACTS                              │  │
│  │                                                                               │  │
│  │  ┌─────────────────────────────────────────────────────────────────────────┐  │  │
│  │  │                      Core TimeBank Contract                             │  │  │
│  │  │  • timeCredits mapping (address => uint256)    // Balances "Table"      │  │  │
│  │  │  • earn() function                                                      │  │  │
│  │  │  • spend() function                                                     │  │  │
│  │  │  • donate() function                                                    │  │  │
│  │  │  • poolPayout() function                                                │  │  │
│  │  └─────────────────────────────────────────────────────────────────────────┘  │  │
│  │                                                                               │  │
│  │  ┌─────────────────────────────────────────────────────────────────────────┐  │  │
│  │  │                      Token Contract (ERC-20 / ERC-721)                  │  │  │
│  │  │  • TimeCreditToken (ERC-20) for fungible time credits                   │  │  │
│  │  │  • ServiceNFT (ERC-721) for unique service offerings                    │  │  │
│  │  └─────────────────────────────────────────────────────────────────────────┘  │  │
│  │                                                                               │  │
│  │  ┌─────────────────────────────────────────────────────────────────────────┐  │  │
│  │  │                      Event Logs (On-Chain History)                      │  │  │
│  │  │  event TimeEarned(address user, uint256 minutes, uint256 timestamp)     │  │  │
│  │  │  event TimeSpent(address from, address to, uint256 minutes, ...)        │  │  │
│  │  │  event TimeDonated(address from, address pool, uint256 minutes, ...)    │  │  │
│  │  │  event PoolPayout(address pool, address to, uint256 minutes, ...)       │  │  │
│  │  └─────────────────────────────────────────────────────────────────────────┘  │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
│                                              │                                      │
│              ┌───────────────────────────────┼───────────────────────────────┐      │
│              ▼                               ▼                               ▼      │
│  ┌───────────────────────┐   ┌───────────────────────────┐   ┌─────────────────────┐│
│  │      Ethereum         │   │         Polygon           │   │   Cross-Chain       ││
│  │      Network          │   │         Network           │   │   Bridge            ││
│  │  (Mainnet / Testnet)  │   │   (Mainnet / Testnet)     │   │   (Future)          ││
│  └───────────────────────┘   └───────────────────────────┘   └─────────────────────┘│
└─────────────────────────────────────────────────────────────────────────────────────┘
                                              │
                                              ▼
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                           INTEROPERABILITY & GOVERNANCE LAYER                       │
│                                    (Future)                                         │
│                                                                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                      Cross-Community Interoperability                         │  │
│  │  ┌─────────────────────────┐         ┌─────────────────────────────────────┐  │  │
│  │  │ Global Timebank Registry│         │  Cross-Border Exchange Protocol     │  │  │
│  │  │  • Community Discovery  │         │  • Atomic Swaps                     │  │  │
│  │  │  • Trust Scoring        │         │  • Exchange Rate Oracle             │  │  │
│  │  └─────────────────────────┘         └─────────────────────────────────────┘  │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
│                                                                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                         DAO Governance Layer                                  │  │
│  │  ┌─────────────────────────┐         ┌─────────────────────────────────────┐  │  │
│  │  │  Governance Token       │         │  Voting Mechanism                   │  │  │
│  │  │  (Time Credit based)    │         │  • Proposal Creation                │  │  │
│  │  └─────────────────────────┘         │  • Quadratic Voting                 │  │  │
│  │                                      │  • Dispute Resolution               │  │  │
│  │  ┌─────────────────────────┐         └─────────────────────────────────────┘  │  │
│  │  │  Treasury Management    │                                                  │  │
│  │  │  • Community Fund       │                                                  │  │
│  │  │  • Upgrade Proposals    │                                                  │  │
│  │  └─────────────────────────┘                                                  │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────────────────────────────┘
                                              │
                                              ▼
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                              ANALYTICS & INSIGHTS LAYER                             │
│                                                                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                         Community Analytics Platform                          │  │
│  │                                                                               │  │
│  │  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────────────────────┐│  │
│  │  │  Engagement     │  │  Impact         │  │  Demand Forecasting             ││  │
│  │  │  Dashboards     │  │  Metrics        │  │  • AI-powered predictions       ││  │
│  │  │  • Active users │  │  • Hours pooled │  │  • Skill gap analysis           ││  │
│  │  │  • Tx volume    │  │  • Communities  │  │  • Resource optimization        ││  │
│  │  └─────────────────┘  └─────────────────┘  └─────────────────────────────────┘│  │
│  │                                                                               │  │
│  │  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────────────────────┐│  │
│  │  │  Reputation     │  │  Network        │  │  Personalized                   ││  │
│  │  │  Leaderboard    │  │  Graph          │  │  Recommendations                ││  │
│  │  │  • Trust scores │  │  • Connections  │  │  • Skill matches                ││  │
│  │  │  • Badges       │  │  • Clusters     │  │  • Opportunity alerts           ││  │
│  │  └─────────────────┘  └─────────────────┘  └─────────────────────────────────┘│  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────────────────────────────┘</pre>

**JeffreyWoo TimeBank** is currently a conceptual DApp built on a blockchain‑inspired hash‑chained ledger. Future development may extend this foundation into a fully deployed smart contract ecosystem. Planned directions include:

- **Smart Contract Deployment**

  - Implement core time credit logic in Solidity  
  - Deploy contracts to Ethereum or Polygon for transparent, verifiable exchanges

- **Tokenization of Time Credits**

  - Represent each hour of service as a transferable ERC‑20 or ERC‑721 token  
  - Enable interoperability with other decentralized applications

- **Decentralized Identity (DID) Integration**

  - Support verifiable digital identities for participants  
  - Build reputation scoring based on contribution history

- **AI‑Enhanced Matching Engine**

  - Expand skill‑matching algorithms with advanced AI APIs  
  - Optimize community exchanges by predicting demand and supply trends

- **Cross‑Community Interoperability**

  - Connect multiple local timebanks into a global network  
  - Enable cross‑border exchanges of time credits

- **Governance & Data Access Object (DAO) Model**

  - Introduce community voting for rules, upgrades, and dispute resolution  
  - Ensure democratic participation in platform evolution

## 📦 Getting Started

1.	Clone the repository
    ```
  	git clone https://github.com/wcfjeffrey/jeffreywoo-timebank-dapp.git  
    cd jeffreywoo-timebank-dapp
    ```
    
2.	Install dependencies  
    `npm install`
  	
3.	Set up environment variables  
    Create .env.local and add your keys:  
    ```
    GEMINI_API_KEY=your_api_key_here
    BLOCKCHAIN_NETWORK=polygon
    ```
    
4.	Run the app  
    `npm run dev`

## 🧠 Sample

<img src="assets/JeffreyWooTimeBank1.png" alt="JeffreyWooTimeBank1" width="1200" height="1000" />
<img src="assets/JeffreyWooTimeBank2.png" alt="JeffreyWooTimeBank2" width="300" height="600" /> 
<img src="assets/JeffreyWooTimeBank3.png" alt="JeffreyWooTimeBank3" width="300" height="600" /> 
<img src="assets/JeffreyWooTimeBank4.png" alt="JeffreyWooTimeBank4" width="1200" height="1200" />

### ⛓️ Blockchain Mechanism Illustrated by a Ledger Example

<img src="assets/JeffreyWooTimeBank4a.png" alt="JeffreyWooTimeBank4a" width="1200" height="600" />

Priya Iyer offers a 30‑minute portfolio + resume review for designers via video call.

The previous transaction’s hash is:  
- PrevHash: 300cd5...d8ac  
- EntryHash (computed): f31ab3...317e

#### 📋 Transaction Fields

|Field	|Value|
|-------|-----|
|ID	|tx2001|
|Index	|1|
|Kind	|GRANT|
|From ID	|user123|
|From Name	|Priya Iyer|
|To ID	|user789|
|To Name	|Designer Participant|
|Minutes	|30|
|Memo	|Portfolio + resume review|
|Related Service ID	|svc456|
|Related Service Title	|30-min video call feedback|
|Created At	|2026-04-22T10:00:00Z|
|PrevHash	|300cd5...d8ac|

#### 🧮 Hash Payload Construction

To compute the **entryHash**, I concatenate the fields into a single string:
```
tx2001|1|GRANT|user123|Priya Iyer|user789|Designer Participant|30|Portfolio + resume review|svc456|30-min video call feedback|2026-04-22T10:00:00Z|300cd5...d8ac
```

#### 🔐 Hash Computation

Using **SHA‑256**:
```
import crypto from "crypto";

function computeHash(data: string) {
  return crypto.createHash("sha256").update(data).digest("hex");
}

const payload = "tx2001|1|GRANT|user123|Priya Iyer|user789|Designer Participant|30|Portfolio + resume review|svc456|30-min video call feedback|2026-04-22T10:00:00Z|300cd5...d8ac";

const entryHash = computeHash(payload);
console.log(entryHash); // f31ab3...317e
```

#### 📘 How Blockchain Works

**1. Transaction A (prevHash: before Priya’s entry)**

- Its fields are concatenated into a payload string.  
- SHA‑256 hashing produces `entryHash_A` = 300cd5...d8ac.

**2. Transaction B (entryHash_B: Priya’s entry)**

- Includes `prevHash` = `entryHash_A`.  
- Concatenates all fields **including that `prevHash` into a new payload**.  
- Hashing this payload produces `entryHash_B` = f31ab3...317e.

**3. Dependency**

- Priya’s `entryHash_B` is valid only if the `prevHash` matches the actual hash of the previous transaction.  
- If Transaction A were altered, its `entryHash_A` would change, breaking the link in Transaction B.

#### ✅ Result

- **PrevHash:** 300cd5...d8ac  
- **EntryHash:** f31ab3...317e
- Each entryHash locks in the previous transaction’s hash.
- This creates a hash‑chained ledger: TxA → TxB → TxC …
- Any tampering in earlier entries invalidates all subsequent hashes, ensuring immutability and transparency.

This demonstrates how Priya Iyer’s **30‑minute video call review** is cryptographically linked to the previous transaction. Any change in the fields (e.g., minutes, memo, or names) would alter the entryHash, breaking the chain and ensuring tamper‑evidence.

<img src="assets/JeffreyWooTimeBank5.png" alt="JeffreyWooTimeBank5" width="1200" height="1000" /> 
<img src="assets/JeffreyWooTimeBank6.png" alt="JeffreyWooTimeBank6" width="1200" height="600" /> 
<img src="assets/JeffreyWooTimeBank7.png" alt="JeffreyWooTimeBank7" width="1200" height="600" />
<img src="assets/JeffreyWooTimeBank8.png" alt="JeffreyWooTimeBank8" width="1200" height="1000" /> 
<img src="assets/JeffreyWooTimeBank9.png" alt="JeffreyWooTimeBank9" width="1200" height="600" /> 
<img src="assets/JeffreyWooTimeBank10.png" alt="JeffreyWooTimeBank10" width="1200" height="600" />
<img src="assets/JeffreyWooTimeBank11.png" alt="JeffreyWooTimeBank11" width="1200" height="600" /> 
<img src="assets/JeffreyWooTimeBank12.png" alt="JeffreyWooTimeBank12" width="1200" height="600" /> 
<img src="assets/JeffreyWooTimeBank13.png" alt="JeffreyWooTimeBank13" width="1200" height="600" />
<img src="assets/JeffreyWooTimeBank14.png" alt="JeffreyWooTimeBank14" width="500" height="400" /> 
<img src="assets/JeffreyWooTimeBank15.png" alt="JeffreyWooTimeBank15" width="1200" height="600" /> 
 
*Note: Both earn and spend/donate time credits transparently through the DApp. AI recommends future matches based on skill compatibility and community needs.*

## ⚖️ Disclaimer

**JeffreyWoo TimeBank** is a conceptual decentralized application created for **educational, research, and community development purposes only**. It is not intended to function as a financial product, investment vehicle, or regulated service. The platform does not issue, trade, or guarantee monetary assets, and any time credits exchanged within the system are purely illustrative and non‑financial. Use of this project should be understood as experimental and exploratory, without any implication of financial return, legal enforceability, or commercial offering.

## 📄 License

**Proprietary License** — JeffreyWoo TimeBank

This repository and its contents are proprietary to JeffreyWoo TimeBank.

Unauthorized copying, modification, distribution, or use of the code, documentation, or related materials is strictly prohibited without prior written consent.

## 👤 About the Author
Jeffrey Woo — Finance Manager | Strategic FP&A, AI Automation & Cost Optimization | MBA | FCCA | CTA | FTIHK | SAP Financial Accounting (FI) Certified Application Associate | Xero Advisor Certified

📧 Email: jeffreywoocf@gmail.com  
💼 LinkedIn: https://www.linkedin.com/in/wcfjeffrey/  
🐙 GitHub: https://github.com/wcfjeffrey/
