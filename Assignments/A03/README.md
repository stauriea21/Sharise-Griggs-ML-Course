# A03 – Case Study: Edge-Computing Video Analytics for Real-Time Traffic Monitoring

**Course:** ITAI 3377 – A.I. at the Edge & IIoT Environments  
**Student:** Sharise Griggs  
**Score:** 91/100

---

## Problem Statement

This assignment critically analyzed the Liverpool Smart Pedestrians project — a real-world smart city deployment that used edge computing and computer vision to monitor pedestrian and vehicle movement in Liverpool, Australia, without storing or transmitting raw video footage.

---

## My Approach

I wrote a structured report covering all required sections: project objectives, methodology, technology stack, validation results, real-world applications, challenges, and a personal evaluation. I connected the project's design decisions back to course concepts from Module 2 (edge computing) and Module 3 (sensor networks and edge gateways).

---

## Key Technical Concepts Covered

- NVIDIA Jetson TX2 as an embedded AI inference platform
- YOLOv3 for real-time multi-object detection
- SORT algorithm (Kalman filtering) for object tracking
- Privacy-by-design: only metadata transmitted, no raw video stored
- Distributed edge architecture with 20 deployed sensors across Liverpool

---

## Key Findings

- Edge-based inference enables real-time mobility analytics while preserving citizen privacy
- The system's biggest limitation was reduced accuracy in high-density crowded scenes due to occlusion
- Advancements since 2019 such as YOLOv8, Jetson Orin, 5G, and federated learning would meaningfully improve this type of system
- Predictive analytics layered on top could shift planners from reactive to proactive infrastructure decisions

---

## Files

| File | Description |
|------|-------------|
| `A03_Griggs_Sharise_ITAI_3377.pdf` | Full case study analysis report |
