# Capstone Project – SmartForge ForgeGuard Autonomous Agent

**Course:** ITAI 3377 – A.I. at the Edge & IIoT Environments  
**Student:** Sharise Griggs | Individual Submission – Conceptual Path  
**Due Date:** April 29, 2026

---

## Project Overview

ForgeGuard is a conceptually designed autonomous AI agent for SmartForge, a hypothetical smart manufacturing facility. The agent uses Generative Adversarial Networks (GANs) and reinforcement learning to predict and prevent machine failures before they occur — reducing unplanned downtime and cutting unnecessary maintenance costs.

---

## Path Chosen

Conceptual Path — Full system blueprint and architecture document. No live coding required.

---

## System Architecture

| Layer | Components |
|-------|------------|
| Device Layer | Vibration sensors, temperature probes, CNC machines, power monitors |
| Edge Layer | TensorFlow Lite models deployed on NVIDIA Jetson and Raspberry Pi nodes |
| AI and Decision Layer | GAN for synthetic failure data generation plus RL-based decision engine |

**Communication:** MQTT over TLS 1.3 (sensor to edge), HTTPS/REST (edge to cloud)  
**Security:** OAuth 2.0, AES-256 encryption, role-based access control

---

## Generative AI Approach

A GAN (Generative Adversarial Network) solves the rare-failure training problem in manufacturing. Since real machine failures are uncommon, the GAN generates realistic synthetic failure signals that the predictive model can learn from — without waiting for actual breakdowns to occur.

---

## Autonomous Decision-Making

ForgeGuard combines two approaches:
- Rule-based triggers: Immediate response to threshold violations such as a vibration spike
- Reinforcement learning: Learns over time which maintenance decisions minimize downtime, cost, and disruption

---

## Security and Ethics

- Secure by Design: TLS 1.3, MFA, anomaly detection, and model poisoning prevention built in from the start
- Explainability dashboard so operators understand every autonomous decision ForgeGuard makes
- Worker privacy: all sensor data is machine-only and personally identifiable behavior is excluded

---

## Testing Plan (Theoretical)

| Test | Goal |
|------|------|
| Stress Test | Handle 10x normal data volume without data loss |
| Security Breach Simulation | Verify TLS and OAuth hold under attack |
| Model Accuracy Test | 90% or higher accuracy on injected failure signatures |
| Failover Test | Full autonomous operation with cloud connectivity cut |

---

## Files

| File | Description |
|------|-------------|
| `CP_ShariseGriggs_Individual_ITAI_3377_ConceptualDoc.docx` | Full conceptual development document |
| `CP_ShariseGriggs_Individual_ITAI_3377_Presentation.pptx` | Capstone presentation slides |
