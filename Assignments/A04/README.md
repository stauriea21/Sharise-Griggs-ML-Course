# A04 – Reflective Journal: IIoT Protocols Project

**Course:** ITAI 3377 – A.I. at the Edge & IIoT Environments  
**Student:** Sharise Griggs  
**Score:** 94/100

---

## What This Assignment Covers

This individual reflective journal documents my experience completing Lab 04 — simulating an IIoT sensor network using three industrial communication protocols: MQTT, CoAP, and OPC UA. I worked as part of Group 5.

---

## My Contributions

- Led environment setup on Windows including virtual environment configuration and Mosquitto broker installation as a Windows Service
- Wrote and debugged the MQTT sensor simulation and visualization scripts
- Resolved a Windows-specific threading error by restructuring the visualization to use FuncAnimation on the main thread
- Contributed to the written protocol comparison report

---

## What I Learned

| Protocol | Key Insight |
|----------|-------------|
| MQTT | Publish/subscribe model allows decoupled, scalable device communication |
| CoAP | UDP-based, RESTful feel — ideal for power-constrained edge devices |
| OPC UA | Full data modeling system with structured hierarchy — the protocol industrial machines actually use |

---

## Challenges Solved

- MQTT threading error: RuntimeError Calling Tcl from different apartment — fixed by separating the MQTT network loop from chart updates using FuncAnimation
- CoAP port conflict: Used netstat and taskkill to identify and clear port 5683
- OPC UA async/await syntax error: Removed incorrect await on a synchronous property after reading library documentation

---

## Key Takeaway

There is no single best protocol — the right choice depends on the environment, the device constraints, and how much structure the data needs. Knowing when to use which one is the real skill.

---

## Files

| File | Description |
|------|-------------|
| `A04_Griggs_Sharise_ITAI_3377.pdf` | Individual reflective journal |
