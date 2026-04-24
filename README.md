<div align="center">
  <img src="assets/JeffreyWooTimeBank.png" alt="JeffreyWooTimeBankBanner" width="1200" height="600" />
</div>

## 📊 Overview
         
> **Not your typical community exchange app!**

**JeffreyWoo TimeBank** is a decentralized, AI-powered timebanking DApp that enables communities to exchange skills, services, and care using time credits as currency. Built on a blockchain-inspired, hash-chained ledger, every transaction is cryptographically linked, tamper-resistant, and publicly verifiable — ensuring trust without intermediaries.  

AI-driven matching intelligently connects neighbors by skills and needs, fostering collaboration across generations and professions. The principle is simple yet powerful: **1 hour given = 1 hour earned**. By combining transparent ledger technology with adaptive AI, it transforms volunteering into a sustainable, equitable ecosystem where time itself becomes the foundation of community value.

## ✨ What It Does

🤝 **Community Time Exchange** — trade time and skills directly with others through smart contracts  
🧠 **AI Matching Engine** — intelligently connects users based on skill profiles, availability, and community needs  
🔗 **Blockchain Transparency** — ensures secure, immutable records of time transactions  
🌍 **Global & Local Integration** — supports Hong Kong community exchanges while connecting to global timebank networks  
🔒 **Digital Identity & Trust Layer** — verifies participants via decentralized identity (DID) and reputation scoring

## 💡 Social Impact

This project demonstrates how technology can reshape community collaboration by:  
- Empowering individuals to value time equally, regardless of profession or income
- Building trust through transparent, decentralized time exchange
- Encouraging social inclusion and intergenerational cooperation
- Promoting sustainable community development through equitable resource sharing
- Integrating AI to optimize skill matching and time utilization

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

## 🏗️ System Architecture Overview
<pre lang="markdown">
               ┌───────────────────────────┐
               |   User Interface (React)  |
               |   TypeScript Frontend     |
               └───────────────────────────┘
                            ↓
               ┌───────────────────────────┐
               |   Frontend Logic          |
               |   State Mgmt / API Calls  |
               └───────────────────────────┘
                             |
             ┌─────────────────────────────────┐
             ↓                                 ↓
     ┌────────────────┐         ┌───────────────────────────┐
     | Smart Contracts|         | AI Matching Engine        |
     | (Solidity)     |         | Gemini API / GPT-4o       |
     |                |         | (Pluggable AI Model APIs) |
     └────────────────┘         └───────────────────────────┘
              ↓                                ↓
┌───────────────────────────┐   ┌───────────────────────────┐
| Blockchain Network        |   | Skill & Profile Database  |
| Ethereum / Polygon        |   | PostgreSQL / Redis        |
| (Configured chain)        |   |                           | 
└───────────────────────────┘   └───────────────────────────┘
              ↓                                ↓
┌───────────────────────────┐   ┌───────────────────────────┐
| Transaction Ledger        |   | Community Analytics       |
| Immutable Records         |   | Dashboards & Insights     |
└───────────────────────────┘   └───────────────────────────┘</pre>

## 🤖 Tech Stack

- **Language:** TypeScript, HTML
- **Framework:** React (Next.js optional)
- **Backend:** Node.js + FastAPI (for AI integration)
- **Blockchain:** Ethereum / Polygon (Smart Contracts via Solidity)
- **AI Models:** Gemini API, ChatAnywhere GPT 4o ca
- **Database:** PostgreSQL, Redis
- **UI:** Tailwind CSS + Recharts + Framer Motion

## 🔗 Blockchain & Ledger Technology

**JeffreyWoo TimeBank** leverages a hash‑chained ledger architecture inspired by blockchain principles to ensure trust, transparency, and accountability in time credit exchanges.

**Core Features**

- **Hash‑Chained Transactions**

Every service exchange is recorded as a transaction linked cryptographically to the previous one, forming an immutable chain of records.

- **Public Verifiability**

Transactions are auditable and tamper‑resistant, ensuring community trust without requiring centralized intermediaries.

- **Time Credits as Currency**

Each hour of service provided equals one hour earned. Credits circulate freely, enabling flexible exchanges across the community.

- **AI‑Enhanced Matching**

AI algorithms connect participants by skills and needs, ensuring efficient and equitable distribution of time credits.

- **Decentralized Identity & Reputation**

Each participant maintains a verifiable digital identity, with reputation scores built from contribution history.

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

## 🪙 Future Roadmap

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

- **Governance & DAO Model**

  - Introduce community voting for rules, upgrades, and dispute resolution  
  - Ensure democratic participation in platform evolution

## 📦 Getting Started

1.	Clone the repository
    ```
  	git clone `https://github.com/wcfjeffrey/jeffreywoo-timebank-dapp.git  
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

### 🔗 Blockchain Explanation by A Sample Ledger Entry

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

To compute the **entryHash**, we concatenate the fields into a single string:
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

#### ✅ Result

- **PrevHash:** 300cd5...d8ac
- **EntryHash:** f31ab3...317e

This demonstrates how Priya’s **30‑minute video call review** is cryptographically linked to the previous transaction. Any change in the fields (e.g., minutes, memo, or names) would alter the entryHash, breaking the chain and ensuring tamper‑evidence.

<img src="assets/JeffreyWooTimeBank5.png" alt="JeffreyWooTimeBank5" width="1200" height="1000" /> 
<img src="assets/JeffreyWooTimeBank6.png" alt="JeffreyWooTimeBank6" width="1200" height="600" /> 
<img src="assets/JeffreyWooTimeBank7.png" alt="JeffreyWooTimeBank7" width="1200" height="600" />
<img src="assets/JeffreyWooTimeBank8.png" alt="JeffreyWooTimeBank8" width="1200" height="1000" /> 
<img src="assets/JeffreyWooTimeBank9.png" alt="JeffreyWooTimeBank9" width="1200" height="600" /> 
<img src="assets/JeffreyWooTimeBank10.png" alt="JeffreyWooTimeBank10" width="1200" height="600" />
<img src="assets/JeffreyWooTimeBank11.png" alt="JeffreyWooTimeBank11" width="1200" height="600" /> 
<img src="assets/JeffreyWooTimeBank12.png" alt="JeffreyWooTimeBank12" width="1200" height="600" /> 
<img src="assets/JeffreyWooTimeBank13.png" alt="JeffreyWooTimeBank13" width="1200" height="600" />
<img src="assets/JeffreyWooTimeBank14.png" alt="JeffreyWooTimeBank14" width="600" height="400" /> 
<img src="assets/JeffreyWooTimeBank15.png" alt="JeffreyWooTimeBank15" width="1200" height="600" /> 
 
*Note: Both earn and spend time credits transparently through the DApp. AI recommends future matches based on skill compatibility and community needs.*

## ⚖️ Disclaimer

**JeffreyWoo TimeBank** is a conceptual decentralized application created for **educational, research, and community development purposes only**. It is not intended to function as a financial product, investment vehicle, or regulated service. The platform does not issue, trade, or guarantee monetary assets, and any time credits exchanged within the system are purely illustrative and non‑financial. Use of this project should be understood as experimental and exploratory, without any implication of financial return, legal enforceability, or commercial offering.

## 📄 License

**GNU Affero General Public License v3.0 (AGPL‑3.0)** — JeffreyWooFinance 

- ✅ You are free to use, modify, and distribute this software, provided that any derivative works are also licensed under AGPL‑3.0.
- ✅ If you run or deploy this software over a network (e.g., as a web service), you must make the source code of your modified version available to all users who interact with it.
- ✅ This ensures transparency, collaboration, and continued open‑source availability of improvements.
- ❌ The software is provided “as is”, without warranties of any kind.

For full details, see the [LICENSE](./LICENSE) file.

## 👤 About the Author
Jeffrey Woo — Finance Manager | Strategic FP&A, AI Automation & Cost Optimization | MBA | FCCA | CTA | FTIHK | SAP Financial Accounting (FI) Certified Application Associate | Xero Advisor Certified

📧 Email: jeffreywoocf@gmail.com  
💼 LinkedIn: https://www.linkedin.com/in/wcfjeffrey/  
🐙 GitHub: https://github.com/wcfjeffrey/
