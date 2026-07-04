# 🛡️ SPECTOR INTERACTION SYSTEM
### Universal Anti-Cybercrime & Threat Intelligence Platform

Spector is a production-grade, cloud-hosted **Pre-Execution Threat Intelligence Suite**. Featuring a custom, high-fidelity dark enterprise interface, it allows everyday internet users and security administrators to scan live URLs, malicious binary payloads, and current-era financial scams before execution. 

The platform strips asset layers and dynamically cross-references them against active cybercrime infrastructure signatures, providing instant forensic classification and an **Automated Incident Response (IR) Playbook**.

🌍 **Live Web Portal:** [https://universal-anti-cybercrime-threat-intelligence-myjzketqxngmzcxq.streamlit.app/](https://universal-anti-cybercrime-threat-intelligence-myjzketqxngmzcxq.streamlit.app/)

---

## 🚀 Core Capabilities (What This Project Solves)

Spector operates at the pre-execution layer, stopping cyber attacks before a user clicks a link or opens a downloaded file. It defends against 4 major modern cybercrime vectors:

### 1. Phishing Infrastructure & Reverse Tunneling Detection
* **The Threat:** Attackers deploy automated port-forwarding tools (like `Zphisher` or `HiddenEye`) routed through proxies to clone official enterprise login screens (e.g., GitHub, Instagram, or online banking pages).
* **Spector's Defense:** The engine dynamically parses URLs to flag active proxy tunnels (`ngrok.io`, `serveo.net`, etc.) combined with Brand Spoofing heuristic patterns, preventing credential theft.
* **MITRE ATT&CK Alignment:** `T1566` (Phishing) & `T1583.003` (Acquire Infrastructure: Virtual Tunnels).

### 2. Executable Payload & Malware Deployment Shield
* **The Threat:** Weaponized system scripting files and binaries (`.exe`, `.scr`, `.bat`, `.apk`) disguised as legitimate utility updates, free tools, or invoices to deploy ransomware and info-stealers.
* **Spector's Defense:** The framework scans string arrays for hidden execution extensions, immediately triggering critical containment warnings.
* **MITRE ATT&CK Alignment:** `T1204.002` (User Execution: Malicious File) & `T1059` (Command and Scripting Interpreter).

### 3. Current-Era Web3 Capital Theft & Crypto Frauds
* **The Threat:** High-velocity modern financial frauds, including malicious smart-contract triggers, lookalike cryptocurrency exchanges, and fake WhatsApp/Telegram airdrop scams designed to drain digital wallets.
* **Spector's Defense:** Performs heuristic keyword matching against modern token fraud signatures to block Web3 credential compromise.

### 4. Transport Security & Cleartext Compliance
* **The Threat:** Data transmitted over standard HTTP channels, making it fully vulnerable to Man-In-The-Middle (MITM) wiretapping.
* **Spector's Defense:** Evaluates the encryption state of incoming assets and prompts users to enforce secure TLS/HTTPS channels.

---

## 🎨 Enterprise UI/UX Architecture

Spector features a **Cyberpunk-Style Security Dashboard** utilizing custom embedded CSS injections to maximize operational visibility:

1. **Central Threat Terminal:** A clean, centralized utility command box where users can input any untrusted digital asset for an instant audit.
2. **Forensic Intelligence Panel (Left Column):** Upon detecting a malicious threat signature, the engine prints a structural breakdown explaining *why* the asset was flagged.
3. **Incident Response Protocol (Right Column):** Rather than throwing a basic error message, it acts as an automated **SOC Analyst**, providing custom step-by-step mitigation instructions (e.g., disconnecting network adapters, session resets, or proxy abuse reporting).

---

## 🛠️ Technology Stack & Implementation Logic

* **UI Layer:** Python 3.14 + Streamlit Web Architecture (Custom Enterprise UI Styles).
* **Logic Core:** Regular Expressions (Regex), `urllib.parse` URI segment parsing, and array evaluation heuristics.
* **DevOps Pipeline:** Git-triggered CI/CD orchestration. Pushing code directly to the GitHub main branch automates production updates on the Streamlit Community Cloud without manual re-deployment.

---

## 📊 Threat Simulation Matrix (How to Test)

Any reviewer or user can benchmark the live detection engine by entering the following simulation strings into the portal:

| Input Asset String | Target Cybercrime Core | Expected System Output |
| :--- | :--- | :--- |
| `http://verify-github-login.ngrok.io` | 🛑 Phishing & Credential Theft via Proxy | Red Critical Alert + Zphisher Forensic Mitigation Steps |
| `secure_invoice_report.scr` / `patch.exe` | 🛑 Malware / Ransomware Execution Threat | Red Critical Alert + System Isolation Playbook |
| `http://claim-free-bitcoin-bonus.com` | 🛑 Web3 Financial Wallet Fraud | Red Critical Alert + Wallet Safety Guard |
| `http://my-unsecured-blog.com` | ⚠️ Insecure Transport (HTTP Warning) | Orange Compliance Alert Banner |

---

## 👤 Maintainer Profile
* **Focus:** Security Operations (SOC), Threat Intelligence (CTI), Cloud Automation, and Defensive Security Utilities.
* **Project Status:** Production Ready / Open for Evaluation.
