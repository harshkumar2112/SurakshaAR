<div align="center">

# 🛡️ SurakshaAR

### Augmented Reality Personal Safety & Emergency Navigation System

*AI + AR–Powered Real-Time Hazard Detection & Spatial Safety Ecosystem*

[![LIVE DEMO](https://img.shields.io/badge/🌐_-DOCS-blue?style=for-the-badge)](https://github.com/harshkumar2112/SurakshaAR)
[![DOCUMENTATION](https://img.shields.io/badge/🌐_LIVE-DEMO-blue?style=for-the-badge)](#)
[![AR ENGINE](https://img.shields.io/badge/🕶️_AR-FOUNDATION-purple?style=for-the-badge)](https://unity.com/)
[![AI POWERED](https://img.shields.io/badge/🤖_AI-YOLOV8-red?style=for-the-badge)](https://github.com/ultralytics/ultralytics)

---

</div>

## Project Overview

The **SurakshaAR Personal Safety System** revolutionizes urban safety by combining Augmented Reality (AR) spatial overlays with AI-driven hazard detection. The system dynamically overlays real-time safe navigation paths on live camera feeds, detects threats in low-light environments, provides automated SOS alerting with spatial coordinates, and connects users to nearby safe havens and verified response teams.

<br>

## Key Features

**AR Spatial Navigation** - Real-time visual directional pathfinding projected onto live environments

**Real-time Visual Hazard Detection** - AI-based threat, unlit zone, and obstacle detection using YOLOv8

**One-Tap & Gesture SOS** - Rapid spatial coordinate transmission to emergency contacts and authorities

**Smart Safe Haven Radar** - AR-anchored indicators for nearby police stations, hospitals, and active safe zones

**Geofenced Crime Heatmaps** - Spatial safety scoring based on historical and real-time community incident data

**Encrypted Live Stream Escort** - Real-time spatial tracking and telemetry sharing for trusted contacts

**Offline-First Incident Logging** - Local coordinate and alert queuing to maintain function during weak signal loss

**Hands-Free Audio Warnings** - Dynamic voice and spatial audio cues guiding users through dark or risky corridors

<br>

---

## System Architecture

```text
+-----------------------------------------------------------------+
|                     SURAKSHAAR ECOSYSTEM                        |
+-----------------------------------------------------------------+
|                                                                 |
|   +----------+  +----------+  +----------+  +----------+        |
|   | Citizen  |  | Emergency|  | Security |  |  Admin   |        |
|   | App (AR) |  | Contacts |  | Responders| | Console  |        |
|   +----+-----+  +----+-----+  +----+-----+  +----+-----+        |
|        |             |             |             |              |
+--------+-------------+-------------+-------------+--------------+
|                      BACKEND SERVICES                           |
+-----------------------------------------------------------------+
|  * Spatial Path Finding      * Hazard Detection Engine          |
|  * SOS Broadcast Engine      * Geospatial Risk Scoring          |
|  * Encrypted Telemetry       * Authentication & Access Control  |
+-----------------------------------------------------------------+
|                        DATA LAYER                               |
+-----------------------------------------------------------------+
|  * Safe Haven Database       * Incident Heatmap Records         |
|  * User Emergency Contacts   * AR Anchors & Point Cloud Cache   |
|  * Live Telemetry Logs       * Audit & Alert Logs               |
+-----------------------------------------------------------------+
### 2. RTV-HD – Real-Time Visual Hazard Detection

**Edge-AI Computer Vision Threat Engine**

An automated low-latency vision pipeline detecting unlit corridors, suspicious objects, and blind corners in real-time.

#### How It Works

```text
Camera Feed -> Low-Light Enhancement -> YOLOv8 Detection -> Threat Classifier -> Spatial Audio Alert -> Event Logging
Threat Level = (Object Proximity Weight) + (Ambient Dark Ratio x Light Factor) + Historical Risk Multiplier
SOS Trigger -> Anchor Capture -> Media Buffer -> WebSocket Transmission -> Responder Alert -> Telemetry Tracking
GPS Scan -> Geofence Filter -> Spatial Node Fetch -> World Anchor Conversion -> Floating Badge Rendering
User Incident Snap -> Metadata Check -> AI Image Verification -> Grid Heatmap Mapping -> Public Warning Push
Unity (AR Foundation / ARCore / ARKit) • C# • Flutter (Companion Mobile App)
Node.js / Python FastAPI • WebSockets • Redis • PostGIS
YOLOv8 • OpenCV • TensorFlow Lite • PyTorch
MongoDB • PostgreSQL (Geospatial Indexes)
Unity Hub >= 2022.3 LTS
Node.js >= 18.x
Python >= 3.9
Android Studio (ARCore Support) / Xcode (ARKit Support)
git clone [https://github.com/harshkumar2112/SurakshaAR.git](https://github.com/harshkumar2112/SurakshaAR.git)
cd SurakshaAR
cd backend
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
cp .env.example .env
python main.py
           ^                      ^                      ^
           |                      |                      |
    [AR Camera Feed]      [Device GPS / IMU]    [Community Reports]
