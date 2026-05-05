# Lab 04 – IIoT Sensor Network & Protocol Experimentation

**Course:** ITAI 3377 – A.I. at the Edge & IIoT Environments  
**Student:** Sharise Griggs | Group 5  
**Score:** 90/100

---

## What This Lab Covers

This lab simulated a full IIoT sensor network in a local Windows environment, implementing and comparing three industrial communication protocols: MQTT, CoAP, and OPC UA. The network generated continuous temperature and humidity sensor data and transmitted it using each protocol.

---

## What We Built

| Protocol | Tools Used | What It Did |
|----------|------------|-------------|
| MQTT | Paho-MQTT, Mosquitto Broker | Published sensor JSON to a topic; visualized live data with matplotlib |
| CoAP | aiocoap (async Python) | Sent POST requests to a local CoAP server; confirmed with 2.04 Changed OK responses |
| OPC UA | asyncua | Exposed a structured SensorDevice object with Temperature and Humidity variables updated every second |

---

## Environment Setup

- Python 3.10 virtual environment on Windows
- Mosquitto MQTT Broker installed as a Windows Service
- Libraries: paho-mqtt, aiocoap, asyncua, matplotlib, pandas, numpy

---

## Challenges Solved

- MQTT threading error on Windows: RuntimeError: Calling Tcl from different apartment — resolved by using FuncAnimation
- CoAP port 5683 conflict: cleared using netstat -ano and taskkill
- OPC UA async/await TypeError: removed incorrect await on a synchronous node property

---

## Key Takeaway

MQTT is quick and flexible. CoAP is RESTful and lightweight. OPC UA carries real industrial weight. Knowing when to use each one is the actual skill — and this lab built that judgment through hands-on experience with all three.

---

## Files

| File | Description |
|------|-------------|
| `Lab04_Griggs_Group5_ITAI3377.pdf` | Lab screenshots and conclusion document |
