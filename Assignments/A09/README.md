# A09 – Individual Case Study Analysis: Autonomous Agents in Industry 4.0

**Course:** ITAI 3377 – A.I. at the Edge & IIoT Environments  
**Student:** Sharise Griggs  
**Score:** 96/100

---

## Problem Statement

Analyze a case study by Leo Hjulstrom on using reinforcement learning to train autonomous AGV (Automated Guided Vehicle) agents to navigate a simulated warehouse environment in an Industry 4.0 context.

---

## My Approach

I wrote a structured analysis covering introduction, implementation, benefits, challenges, and future implications — followed by a personal reflection on how the study changed my understanding of autonomous agents and reward system design.

---

## Key Findings

- Three AGV agents trained using Double Deep Q-Network (DDQN) on a 10x10 grid warehouse simulation over 200,000 episodes
- All 300 assigned tasks completed with zero crashes and zero battery failures — averaging only 2.59 extra steps per task
- Reward design is how you communicate goals to an AI: small step penalties kept agents efficient; large task rewards drove completion

---

## Challenges in the Study

- Simulation only — no real-world testing with human workers or equipment unpredictability
- Simplified battery model with constant drain and instant recharge — not realistic
- Agents had no direct communication — only adjacent-square awareness of other agents
- Reward graphs showed instability common in reinforcement learning when learning new behaviors disrupts existing ones

---

## My Reflection

This case study changed how I think about reinforcement learning. The reward structure is not a technicality — it is the entire design intent of the system. I also appreciated that the author was upfront about what the study did not prove, which is a sign of quality research.

---

## Files

| File | Description |
|------|-------------|
| `A09_Griggs_Sharise_ITAI3377.pdf` | Full case study analysis and reflection |
