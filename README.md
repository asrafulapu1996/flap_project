# 🤖 Robotics and Automation in RMG Manufacturing (FLAP Project)

**Crystal International Group Ltd. | Amigo Bangladesh Ltd.**  
*Industry 4.0 Implementation in Ready-Made Garments (RMG) Manufacturing*

<p align="center">
  <img src="https://img.shields.io/badge/Field-Robotics-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/Industry-4.0-orange?style=flat-square"/>
  <img src="https://img.shields.io/badge/Automation-PLC%2FHMI-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Integration-MES%20%7C%20RCS%20%7C%20WMS-red?style=flat-square"/>
  <img src="https://img.shields.io/badge/AI%20%2B%20Robotics-Smart%20Factory-lightgrey?style=flat-square"/>
</p>

---

## 🧠 Overview

The **FLAP Project** (Factory Logistics Automation Platform) is a flagship **Industry 4.0 initiative** by **Crystal International Group Ltd.**, one of the world’s leading **Ready-Made Garments (RMG)** manufacturers.  
It integrates **robotics**, **industrial automation**, and **digital manufacturing systems** into a unified, intelligent production ecosystem.

After successful implementation in China, FLAP demonstrated:

- 🚀 **40% higher production efficiency**
- ⚙️ Reduced manual labor and human error
- 🔄 Seamless process-to-process information and material flow
- 📈 Enhanced data visibility and traceability

**Amigo Bangladesh Ltd.**, a subsidiary of Crystal Group, is the first facility in Bangladesh to implement this system, representing a major leap toward **smart manufacturing transformation** in the textile industry.

---

## 👨‍🔧 Author & Role

**Md. Asraful Hasan Apu**  
*Senior Robotics & Automation Engineer*  
Crystal International Group Ltd.  

**Responsibilities:**

- Developed intelligent **AGV/AMR systems** for automated material transport using **AI-driven navigation** and **dynamic path planning**.  
- Integrated **robotic arms, elevators, and conveyors** with AGVs for complete material-handling automation.  
- Established **MES–RCS communication** for synchronized process execution.  
- Designed and deployed **PLC/HMI-based subsystems** integrated into the central control framework.  
- Led **cross-functional coordination**, user training, and on-site deployment.  
- Managed **budget and performance optimization** for robotic and automation rollouts.

---

## 🏗️ System Architecture

![Layered Architecture](docs/image/layered-architecture.png)

### 🔹 Multilayer Control Architecture

The FLAP architecture follows a **hierarchical control model**, ensuring seamless data and command flow between enterprise-level decision systems and field-level robotic equipment.

```
Enterprise Layer
 ├── CICS (Central Information & Control System)
 │    ├── MES (Manufacturing Execution System)
 │    ├── WMS (Warehouse Management System)
 │    └── RCS (Robotic Control System)
 │
 └── Control & Orchestration Layer
      ├── Orchestrator / Scheduler (Job allocation, KPI, logging)
      ├── Fleet Manager (AGV task allocation & optimization)
      └── Integration API (OPC-UA / REST / MQTT)

Field Layer
 ├── AGV / AMR Robots (Navigation, local control)
 ├── Robotic Arms (Pick/place, loading)
 ├── PLC/HMI Systems (Local machine control)
 └── Vision Systems (Inspection / QC)

Physical Infrastructure
 ├── Charging Stations
 ├── Conveyors & Elevators
 └── Workstations (Cutting, Spreading, Relaxation, Inspection)
```

**Reference Figures:**
- `docs/image/CICS_Information_Flow.png` — Information hierarchy  
- `docs/image/Overall_Process_Flow.PNG` — Material and data flow  
- `docs/image/System_Process_Flow.png` — Control logic and process coordination  

---

## ⚙️ Process Flow Breakdown

### 🟦 Operation Center
Centralized dashboard for monitoring all robotic and automation systems.  
- `docs/image/Operation_Center_Main_Interface.PNG`  
- `docs/image/Operation_Center_Second_Interface.PNG`

### 🟩 Cutting & Spreading Zone
Automated fabric spreading and cutting managed by the CICS system.  
- `docs/image/Cutting_Task_Allocation_as_per_CICS.jpg`  
- `docs/image/Spreading_Process_User_Interface.jpg`  
- `docs/image/Spreading_Operator_Working.jpg`

### 🟨 Relaxation Zone
Automated relaxation process ensuring consistent fabric handling before cutting.  
- `docs/image/Relaxation_Process_Flow.PNG`  
- `docs/image/Relax_WIP_Monitoring.jpg`  
- `docs/image/Relax_Operator_Working.jpg`

### 🟥 Inspection Zone
AI-based visual inspection for fabric quality and defect detection.  
- `docs/image/Inspection_WorkStaton.jpg`  
- `docs/image/Inspection_Worker_Operationg.jpg`

### 🟧 AGV / AMR Transportation
Autonomous robots perform inter-process material transport and staging.  
- Charging Stations: `docs/image/AGV_Charging_Station_2.jpg`, `docs/image/AGV_Charging_Station_3.jpg`, `docs/image/AGV_Charing_Station.jpg`  
- Empty Trolley Zone: `docs/image/Empty_Trolley_Zone.jpg`

---

## 🔗 System Integration Summary

| Layer | System | Function |
|-------|---------|----------|
| **Enterprise** | CICS | Centralized data and command management |
| **Control** | RCS | AGV task execution and path planning |
| **Execution** | MES | Scheduling and production tracking |
| **Field** | HIKRobot Platform | Hardware integration and sensor data |
| **Human Interface** | Operation Center | Real-time analytics and supervision |

All systems communicate through **TCP/IP** and **OPC-UA**, enabling full interoperability between digital control and robotic execution layers.

---

## 🤖 Robotics and Automation Components

| Component | Description |
|------------|-------------|
| **AGV / AMR Robots** | Autonomous mobile platforms for fabric and WIP transport |
| **RCS (Robotic Control System)** | Multi-robot coordination and navigation control |
| **PLC / HMI Systems** | Local automation for conveyors and mechanical stations |
| **Vision Systems** | AI-based fabric inspection and quality detection |
| **HIKRobot Framework** | Provides vision tracking, sensor data, and localization |
| **CICS Dashboard** | Unified monitoring and analytics across all subsystems |

---

## 📊 Project Outcomes

✅ **40% increase in production throughput**  
✅ **End-to-end digital traceability** of materials  
✅ **Zero manual intervention** in logistics between processes  
✅ **First full FLAP deployment in Bangladesh**  
✅ **Modular design** for scalable Industry 4.0 integration  

---

## 🔬 Research & Innovation Insights

This project demonstrates a **real-world Industry 4.0 architecture** with strong research implications in:

- Multi-robot task allocation and optimization  
- Cyber-physical MES–RCS–AGV integration  
- Vision-based inspection and quality control  
- Intelligent scheduling and dynamic path planning  

### 🧩 Future Research Directions
- **Reinforcement Learning** for AGV decision making under uncertainty  
- **Digital Twin Simulation** for system optimization and predictive analytics  
- **Collaborative Human-Robot Interaction** for mixed-mode operations  

---

## 🖼️ Demonstrations

| Category | Example Interfaces |
|-----------|--------------------|
| **System Monitoring** | `docs/image/RCS_Main_Interface.PNG`, `docs/image/RCS_Statics_Interface.PNG` |
| **Process Flow** | `docs/image/System_Process_Flow.png`, `docs/image/Overall_Process_Flow.PNG` |
| **Automation Zones** | `docs/image/Spreading_User_Interface.jpg`, `docs/image/Inspection_WorkStaton.jpg` |
| **AGV Operations** | `docs/image/AGV_Charging_Station_2.jpg`, `docs/image/AGV_Charging_Station_3.jpg` |

---

## 🚀 Future Expansion

- Integration of **ASRS (Automated Storage & Retrieval System)**  
- Deployment of **robotic manipulators** for automatic loading/unloading  
- Implementation of **predictive maintenance** using AI and analytics  
- Global **cloud synchronization** for centralized production management  

---

## 📚 Citation

If you reference this work in research, reports, or presentations, please cite:

```
Hasan, M. A. (2025). Robotics and Automation in RMG Manufacturing (FLAP Project).  
Crystal International Group Ltd., Amigo Bangladesh Ltd.
```

---

## 📞 Contact

**Md. Asraful Hasan Apu**  
Senior Robotics & Automation Engineer  
Crystal International Group Ltd. | Amigo Bangladesh Ltd.  
📍 Bangladesh  
📧 [Email](mailto:example@email.com) | 🔗 [LinkedIn](#) | 💻 [GitHub](#)

---

<p align="center">
  © 2025 Crystal International Group Ltd. — All Rights Reserved  
</p>
