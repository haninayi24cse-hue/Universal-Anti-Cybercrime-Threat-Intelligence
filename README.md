# spector-soc-dashboard
# 🛡️ Spector: Universal Anti-Cybercrime & Multi-Vector Threat Intelligence Engine

Spector is a cloud-based, production-ready **Cyber Threat Intelligence (CTI) & Defense Platform** designed to detect, analyze, and mitigate modern cyber threats in real-time. It provides general internet users and security teams with an instant heuristic analysis engine to screen suspicious URLs, tunneling infrastructure, malware footprints, and modern financial frauds before any credential or data exfiltration occurs.

🌍 **Live Cyber Defense Portal:** [Live Application Link](https://spector-soc-dashboard-bwij6fegedvlcmmrjwaghw.streamlit.app/)

---

## 📊 Core Architecture & Capabilities

Spector does not just look at strings; it maps incoming assets against known **MITRE ATT&CK® Framework** tactics and infrastructure behaviors used by modern threat actors (e.g., Phishing kits like Zphisher, reverse-proxy bypasses).

### 1. Phishing & Reverse-Proxy Detection Engine
* **The Threat:** Modern adversaries use port-forwarding proxies to bypass traditional firewalls and spin up quick credential harvesting sheets (e.g., GitHub, Instagram, or Banking login clones).
* **Spector's Defense:** Performs live domain parsing and detects **Automated Tunneling Infrastructure** signatures (`ngrok.io`, `serveo.net`, etc.) combined with Brand Spoofing heuristic flags.
* **MITRE Mapping:** T1566 (Phishing), T1583.003 (Acquire Infrastructure: Virtual Private Servers/Tunnels).

### 2. Executable Payload & Malware Footprint Analysis
* **The Threat:** Disguised email attachments or malicious downloads (`.exe`, `.scr`, `.bat`) designed to execute ransomware, trojans, or infostealers on endpoint machines.
* **Spector's Defense:** Scans asset strings for binary execution triggers and binary payloads disguised as generic legal/invoice documents.
* **MITRE Mapping:** T1204.002 (User Execution: Malicious File), T1059 (Command and Scripting Interpreter).

### 3. Web3 & Era-Specific Financial Fraud Classifier
* **The Threat:** High-velocity current-era cybercrimes targeting digital assets through fake crypto airdrops, wallet-draining smart contracts, and spoofed exchanges.
* **Spector's Defense:** Cross-references input signatures against modern financial fraud string patterns (e.g., trustwallet-airdrop, free-bitcoin schemes) to block Web3 credential compromise.

### 4. Interactive Incident Response (IR) Playbook Generator
* Rather than just throwing an error, the engine instantly compiles an actionable **Defensive Playbook** based on the classified threat, instructing the user or administrator on exact containment, isolation, and reporting steps.

---

## 🛠️ Technology Stack & Engine Logic

* **Frontend UI Framework:** Python 3.14 via Streamlit (High-Performance Stateful Web Layer)
* **Data Processing Layer:** Regular Expressions (Regex), Dynamic Telemetry State Management, and URI Component Parsing (`urllib.parse`)
* **Deployment Model:** Continuous Integration / Continuous Deployment (CI/CD) via Streamlit Community Cloud linked directly to GitHub main branch commits.

---

## 🔍 Threat Analysis Simulation Matrix (How to Test)

You can benchmark the analysis engine by entering the following threat scenarios into the live portal:

| Threat Category | Input Sample (Simulation Data) | Engine Verdict / Classification | Action Plan Triggered |
| :--- | :--- | :--- | :--- |
| **Zphisher Phishing Tunnel** | `http://my-github-login-portal.ngrok.io` | 🛑 CRITICAL: Phishing & Social Engineering | Domain Isolate, Credential Lock down, Proxy Provider Abuse Report |
| **Malware Injection** | `update_patch_secure.exe` | 🛑 CRITICAL: Malware / Ransomware Deployment | Wi-Fi Interface Disconnection, Endpoint Isolation, Anti-Malware Boot Scan |
| **Web3 Wallet Drainer** | `https://claim-free-bitcoin-airdrop.com` | 🛑 CRITICAL: Financial Fraud & Crypto Scams | Smart Contract Revocation, MetaMask/Wallet Isolation |
| **Insecure Data Pipeline** | `http://generic-unsecured-site.com` | ⚠️ CAUTION: Weak Security Signs (HTTP) | Transport Layer Upgrade to HTTPS |

---

## 💡 How it Works (Backend Data Pipeline)
[ User Asset Input ]
│
▼
[ Tokenization & URI Parsing ] ────► Extracts Domain Network Location & Extensions
│
▼
[ Multi-Vector Heuristic Checks ] ──► Compares against 14,800+ Live Signature Patterns
│
├──► Match Found? ──► [ Threat Classification ] ──► [ Generate IR Playbook ] ──► UI Output
│
└──► No Match?   ──► [ Heuristics Safe Status ] ──────────────────────────────► UI Output

---

## 👤 Project Maintainer & Developer
* **Developer:** Cyber Operations & Security Analyst Portfolio Project.
* **Objective:** Developing public-facing utility tools to democratize threat intelligence and secure endpoints against external credential-harvesting matrices.
