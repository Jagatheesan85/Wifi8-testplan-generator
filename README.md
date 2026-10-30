# 📡 IEEE 802.11bn (Wi-Fi 8) Test Plan Generator & Validation Suite

![Build Status](https://img.shields.io/badge/IEEE%20802.11bn-UHR%20Ready-00F0FF?style=for-the-badge&logo=wifi)
![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)
![Deployment](https://img.shields.io/badge/Deployment-GitHub%20Pages-blue?style=for-the-badge&logo=github)

An offline, open-source **Test Suite Generator and Validation Architect** tailored for **IEEE 802.11bn Ultra-High Reliability (UHR) / Wi-Fi 8** Access Points and Station MLDs.

Designed specifically for Wireless Quality Assurance Engineers, Test Architects, and Systems Engineers to generate compliance, performance, stability, and stress test vectors directly mapped to draft IEEE 802.11bn MAC/PHY specification clauses.

---

## 🌟 Key IEEE 802.11bn Feature Coverage

This tool covers all key technical pillars defined in the IEEE 802.11bn specification:

- **Multi-AP Coordination (MAPC)**: Coordinated Beamforming (Co-BF), Coordinated Spatial Reuse (Co-SR), Coordinated TDMA (Co-TDMA), and Coordinated Restricted TWT (Co-rTWT).
- **Non-Primary Channel Access (NPCA)**: Dynamic switching to secondary subchannels when primary channel contention occurs.
- **Seamless Mobility Domain (SMD)**: Fast cross-AP MLD context transfer without re-association teardown.
- **Dynamic Subchannel Operation (DSO)**: Per-TXOP subchannel resource allocation beyond client BSS constraints.
- **Distributed Resource Units (dRU)**: Tone spreading over 20/40/80 MHz to maximize uplink PSD limits and range.
- **Enhanced Long Range (ELR)**: Link budget imbalance correction for extended coverage edges.
- **Unequal Modulation (UEQM) & New MCS**: Per-spatial-stream modulation adaptation and fine-grained MCS rates.
- **High-Priority EDCA (P-EDCA)**: Priority contention windows for sub-10ms real-time traffic.

---

## 🚀 Key Tool Capabilities

- **Deep Test Generation**: Generates complete, actionable test plans across 6 core categories:
  - 🛠️ **Functional**: Spec conformance, frame parsing, IE verification.
  - ⚡ **Performance**: 95th percentile latency reduction, throughput scaling, jitter.
  - 🛡️ **Stability**: Long-duration multi-link soak tests, link drop failovers.
  - 🏋️ **Stress**: High-density client queues, control frame flooding.
  - 📐 **Boundary**: Edge MCS, minimum guard intervals, extreme parameter limits.
  - 🔀 **Feature Interaction**: Coexistence between MLO, MAPC, TWT, and P-EDCA.
- **Export Options**: 
  - **PyTest Automation Scripts** (`test_wifi8_suite.py`)
  - **CSV Matrix Export** (`wifi8_test_plan.csv`)
  - **JSON Data Model** (`wifi8_test_plan.json`)
  - **Printable PDF Matrix**

---

## 🛠️ How to Run Locally

Because this project is built as a pure client-side application, **no node server or complex runtime is required**.

### Option A: Direct Browser Launch
1. Clone the repository:
   ```bash
   git clone [https://github.com/your-username/wifi8-testplan-generator.git](https://github.com/your-username/wifi8-testplan-generator.git)
   cd wifi8-testplan-generator
