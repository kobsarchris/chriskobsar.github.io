---
layout: post
title: "Analyzing the 2024 3CX Supply Chain Attack"
date: 2025-04-05 10:00:00 -0400
categories: threat-analysis
---

The 2024 3CX desktop app breach was a **supply chain attack** that compromised thousands of businesses worldwide.

### 🔍 What Happened?
Attackers injected malicious code into a legitimate software update, allowing them to:
- Execute remote code on victim machines
- Steal credentials and session cookies
- Move laterally across networks

### ⚙️ TTPs (MITRE ATT&CK)
- **T1195.002** – Supply Chain Compromise: Software Repositories  
- **T1071.001** – Application Layer Protocol: Web Protocols  
- **T1566** – Phishing

### 🛡️ Detection & Defense
- Monitor for unusual outbound connections (e.g., to unknown IPs)
- Use endpoint detection (EDR) to flag suspicious DLL loads
- Verify software integrity with code signing and SBOMs

### 📌 Why It Matters for Entry-Level Analysts
This attack shows why **trust but verify** is critical — even in trusted vendors. As a SOC or compliance analyst, you must question assumptions and monitor behavior.

🔗 Sources: [The Record](https://therecord.media), [CISA Alert AA23-111A]
