# 🚁 Multi-Modal Drone Detection Using RF Signals and Vision-Based Deep Learning

A portable real-time anti-drone detection system that combines **RF signal analysis** and **AI-powered computer vision** for reliable UAV detection in challenging environments such as border surveillance zones.

The system integrates **RTL-SDR**, **YOLOv8**, **FastAPI**, and a **real-time monitoring dashboard** to improve detection accuracy and reduce false positives.

---

# 📌 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Technologies Used](#️-technologies-used)
- [System Architecture](#-system-architecture)
- [Workflow](#-workflow)
- [Results](#-results)
- [Dashboard Output](#-dashboard-output)
- [Challenges Faced](#️-challenges-faced)
- [Future Work](#-future-work)
- [Applications](#-applications)
- [Contributors](#-contributors)

---

# 📌 Overview

Unauthorized drone activities such as illegal surveillance, smuggling, and security breaches have increased significantly in recent years.

Traditional single-method drone detection systems often fail in:
- Low-visibility environments
- Autonomous drone operations
- Noisy RF conditions
- Cluttered visual backgrounds

This project introduces a **multi-modal sensor fusion approach** combining:

✅ RF Signal Detection using RTL-SDR  
✅ Vision-Based Drone Detection using YOLOv8  
✅ Fusion-Based Decision Engine for enhanced reliability

The system operates in real time and performs efficiently under difficult environmental conditions.

---

# 🚀 Features

- Real-time drone detection
- RF spectrum monitoring using RTL-SDR
- AI-based visual drone detection using YOLOv8
- Fusion-based decision mechanism
- Reduced false positives
- Real-time monitoring dashboard
- Low-latency communication using WebSockets
- Modular and scalable architecture
- Live annotated video feed
- RF spectrum visualization

---

# 🛠️ Technologies Used

## Hardware

- RTL-SDR Module
- Camera Module

## Software & Frameworks

- Python
- YOLOv8
- OpenCV
- FastAPI
- React.js
- Plotly
- WebSockets
- FFT Signal Processing

---

# 🧠 System Architecture

The system consists of two parallel detection pipelines along with a fusion engine.

---

## 1️⃣ RF Detection Module

The RF module captures radio frequency signals from drone communication bands and performs signal analysis.

### Operations Performed

- FFT (Fast Fourier Transform)
- PSD (Power Spectral Density) Analysis
- Peak Detection
- RF Activity Monitoring

### Output

- Detects suspicious RF signal activity
- Identifies potential drone communication patterns

---

## 2️⃣ Vision Detection Module

The vision module processes live camera feed using deep learning.

### Operations Performed

- Real-time video capture
- YOLOv8-based drone detection
- Confidence filtering
- Bounding box annotation

### Output

- Detects drones visually
- Provides confidence score and tracking

---

## 3️⃣ Fusion Engine

The fusion engine combines outputs from RF and vision modules to improve reliability.

| RF Detection | Vision Detection | Output |
|---|---|---|
| Yes | Yes | Confirmed Drone |
| Yes | No | Possible RF Activity |
| No | Yes | Visual Detection |
| No | No | No Threat |

---

# 🔄 Workflow

1. RF signals are captured using RTL-SDR
2. FFT and PSD analysis are performed
3. Camera feed is processed using YOLOv8
4. Detection outputs are sent to the fusion engine
5. Fusion engine validates drone presence
6. Results are displayed on the real-time dashboard

---

# 📊 Results

The proposed fusion-based approach achieved:

✅ Approx. **94% detection accuracy**  

✅ Reduced false positives  

✅ Reliable real-time performance  

✅ Improved robustness in difficult environments  

Experimental testing showed significantly better performance compared to standalone:
- RF-only systems
- Vision-only systems

---

# 📷 Dashboard Output

The dashboard provides:

- Live annotated drone detection feed
- RF spectrum visualization
- Detection status updates
- Real-time monitoring interface
- Alert notifications

---

# ⚠️ Challenges Faced

## Challenges

- RF noise filtering
- Latency during simultaneous processing
- Synchronization between RF and vision modules
- False detections in cluttered backgrounds
- Low-light environmental conditions

## Solutions Implemented

- Threshold filtering
- Confidence validation
- Optimized FFT execution
- Fusion-based asynchronous decision logic
- Improved detection filtering

---

# 🔮 Future Work

Future enhancements may include:

- RF jamming techniques
- GNSS spoofing detection
- Advanced signal manipulation detection
- Edge deployment optimization
- Autonomous drone tracking
- Multi-drone detection support
- Thermal imaging integration

---

# 🌍 Applications

- Border Surveillance
- Military Security
- Airport Protection
- Smart City Monitoring
- Critical Infrastructure Security
- Event Surveillance
- Industrial Zone Protection

---

# 👥 Contributors

- Antara Kumari
- Chaitany Patawari
- Amandeep Singh

---

# 📌 Conclusion

This project demonstrates a robust and scalable **multi-modal anti-drone detection system** that combines RF signal intelligence with AI-powered computer vision.

By integrating:
- RTL-SDR based RF analysis
- YOLOv8 visual detection
- Fusion-based decision making

the system achieves higher reliability, improved detection accuracy, and reduced false positives in real-time surveillance environments.
