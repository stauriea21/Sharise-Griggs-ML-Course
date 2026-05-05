# Midterm – Cybersecurity Plan for an AI-Integrated IIoT System (SmartForge)

**Course:** ITAI 3377 – A.I. at the Edge & IIoT Environments  
**Student:** Sharise Griggs  
**Score:** 92/100

---

## Problem Statement

Design a comprehensive cybersecurity plan for a hypothetical AI-integrated IIoT system — a smart manufacturing facility called SmartForge — covering vulnerability identification, defense strategy development, and penetration testing simulation.

---

## System Overview

SmartForge is a 24/7 precision manufacturing facility using AI-driven predictive maintenance, quality control computer vision, and production scheduling optimization. The system architecture spans four layers: Device, Edge Computing, OT Network, and IT/Cloud.

---

## What I Did

| Section | Content |
|---------|---------|
| Section 1 | Full system design with 6-category vulnerability assessment |
| Section 2 | Defense strategy across 9 domains using Secure by Design principles |
| Section 3 | 4 penetration testing simulations — both attacker and defender roles |
| Section 4 | Final report with key takeaways and proposed improvements |

---

## Vulnerabilities Identified

Device, network, AI model, data, application, and human factor risks — including adversarial inputs, model poisoning, OT/IT segmentation gaps, default credentials, and phishing vectors.

---

## Defense Highlights

- MFA and FIDO2 phishing-resistant authentication for all portals
- TLS 1.3 encryption end-to-end and AES-256 for data at rest
- OT/IT segmentation with data diode and VLAN isolation
- Immutable golden validation dataset to protect the AI retraining pipeline
- SIEM with 12-month log retention and OT-specific intrusion detection

---

## Penetration Test Results

| Scenario | Defense Effectiveness | Key Gap | Fix |
|----------|-----------------------|---------|-----|
| Phishing Attack | High | TOTP MFA bypassable | Upgrade to FIDO2 keys |
| OT Lateral Movement | High | Vendor sessions under-controlled | Add bastion host |
| AI Model Poisoning | Medium | Poisoned validation set | Immutable golden dataset |
| Physical USB Attack | Medium-High | Embedded nodes harder to secure | Tamper-evident seals |

---

## Files

| File | Description |
|------|-------------|
| `MT_Sharise_Solo_ITAI_3377.pdf` | Full cybersecurity plan report |
