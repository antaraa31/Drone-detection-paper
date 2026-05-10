Multi-Modal Drone Detection Using RF Signals and Vision-Based Deep Learning
A portable real-time anti-drone detection system that combines RF signal analysis and AI-powered computer vision for reliable UAV detection in challenging environments such as border surveillance zones. The project integrates RTL-SDR, YOLOv8, FastAPI, and a real-time monitoring dashboard to improve detection accuracy and reduce false positives. 

📌 Overview
Unauthorized drone activities such as illegal surveillance, smuggling, and security breaches have increased significantly in recent years. Traditional single-method drone detection systems often fail in low-visibility environments or when drones operate autonomously.
This project introduces a multi-modal sensor fusion approach that combines:


📡 RF Signal Detection using RTL-SDR


🎥 Vision-Based Drone Detection using YOLOv8


🔀 Fusion-Based Decision Engine for improved reliability


The system is designed to operate in real-time under difficult environmental conditions. 

🚀 Features


Real-time drone detection


RF spectrum monitoring using RTL-SDR


AI-based visual drone detection using YOLOv8


Fusion-based decision mechanism


Reduced false positives


Dashboard for live monitoring


Modular and scalable architecture


Low-latency communication using WebSockets



🛠️ Technologies Used
Hardware


RTL-SDR Module


Camera Module


Laptop / PC Processing Unit


Software & Frameworks


Python


YOLOv8


OpenCV


FastAPI


React.js


Plotly


WebSockets


FFT Signal Processing



🧠 System Architecture
The system works in parallel through two detection pipelines:
1️⃣ RF Detection Module


Captures RF signals from drone communication bands


Performs:


FFT (Fast Fourier Transform)


PSD Analysis


Peak Detection




Identifies suspicious signal activity


2️⃣ Vision Detection Module


Captures real-time video feed


YOLOv8 detects drones visually


Applies confidence filtering and validation


3️⃣ Fusion Engine
Combines outputs from RF and vision modules:
RF DetectionVision DetectionOutputYesYesConfirmed DroneYesNoPossible RF ActivityNoYesVisual DetectionNoNoNo Threat

📊 Results
The proposed fusion-based approach achieved:


✅ Approx. 94% detection accuracy


✅ Reduced false positives


✅ Reliable real-time performance


✅ Improved robustness in difficult environments


Experimental testing showed better performance compared to standalone RF-only or vision-only systems. 

📷 Dashboard Output
The system dashboard includes:


Live annotated drone detection feed


RF spectrum visualization


Detection status updates


Real-time monitoring interface



⚠️ Challenges Faced


RF noise filtering


Latency during simultaneous processing


Synchronization between RF and vision modules


False detections in cluttered backgrounds


Low-light environmental conditions


These challenges were addressed using:


Threshold filtering


Confidence validation


Optimized FFT execution


Fusion-based asynchronous decision logic



🔮 Future Work
Future improvements may include:


RF Jamming techniques


GNSS Spoofing detection


Advanced signal manipulation detection


Edge deployment optimization


Enhanced autonomous drone tracking


