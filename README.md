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
           ^                      ^                      ^
           |                      |                      |
    [AR Camera Feed]      [Device GPS / IMU]    [Community Reports]
```
## Core Modules

### 1. D-ARSN – Dynamic AR Safe Route Navigation

**Priority-Based Safety Route Optimization Algorithm**

A deterministic, real-time spatial pathfinding engine that projects safe directional visual overlays directly onto the user's camera feed to eliminate high-risk navigation.

### How It Works:
```text
Camera Feed -> VIO Tracking -> Spatial Risk Check -> Safety Index Calculation -> Route Ranking -> AR Overlay
```
#### Load Calculation Formula:
```text
Route Safety Score = (Lighting Density x Weight) - (Crime Metric x Risk Factor) + Safe Haven Proximity Bonus
```
#### Path Guidance Rules:
* Highest Safety Path: Green AR Overlay – Optimal lighting, active safe havens

* Moderate Safety Path: Yellow AR Overlay – Average lighting, unverified corridor

* High Risk Corridor: Red AR Block – Dynamic rerouting triggered immediately

#### Benefits:
* Eliminates navigation ambiguity in unfamiliar areas

* Adaptive to real-time community threat data

* Predictable and visual spatial feedback

* Smooth pedestrian and commuter guidance

### 2. RTV-HD – Real-Time Visual Hazard Detection
 
#### Edge-AI Computer Vision Threat Engine
```
An automated low-latency vision pipeline detecting unlit corridors, suspicious objects, and blind corners in real-time.
```
#### How It Works:
```
Plaintext
Camera Feed -> Low-Light Enhancement -> YOLOv8 Detection -> Threat Classifier -> Spatial Audio Alert -> Event Logging
```
#### Threat Level Formula:
```
Plaintext
Threat Level = (Object Proximity Weight) + (Ambient Dark Ratio x Light Factor) + Historical Risk Multiplier
```
#### Detection Levels:
* Critical Threat (Level 3): Immediate AR Bounding Box + Loud Spatial Audio Cue

* Moderate Warning (Level 2): Yellow AR Halo + Dynamic Haptic Vibration

* Low Risk (Level 1): Subtle AR Indicator + Background Heatmap Log

#### Benefits:
* Runs locally on-device using TFLite for minimal latency

* Automatic low-light spatial enhancement

* Proactive hands-free safety warnings

### 3. RS-ED – Rapid SOS & Emergency Dispatch
####Instant Spatial Coordinate Broadcast Ecosystem


A multi-channel emergency alert system transmitting precise 3D spatial anchors, GPS telemetry, and live camera streams to response networks.

#### How It Works:
```
Plaintext
SOS Trigger -> Anchor Capture -> Media Buffer -> WebSocket Transmission -> Responder Alert -> Telemetry Tracking
```
#### Dispatch Workflow:
* Trigger Activation: Screen tap, gesture sequence, or impact acceleration threshold met.

* Payload Encapsulation: Captures 3D world anchor, GPS coordinates, device compass heading, and battery level.

* Emergency Broadcast: Pushes encrypted payload over WebSockets/MQTT to backend dispatch queue.

* Responder Dispatch: Alerts nearest 5 trusted emergency contacts and active security hubs simultaneously.

#### Benefits:
* Sub-second notification dispatch time

* Encrypted live video and spatial audio streaming

* Offline-first queuing automatically re-transmits upon network recovery

 ### 4. SSH-R – Smart Safe Haven Radar
#### Augmented Spatial Anchor Refuge Finder

An AR-anchored radar system identifying verified refuge zones (police posts, 24/7 commercial establishments, hospitals) in the user's immediate environment.

#### How It Works:
```
Plaintext
GPS Scan -> Geofence Filter -> Spatial Node Fetch -> World Anchor Conversion -> Floating Badge Rendering
```
#### Proximity Metrics:
* Under 200m: Direct floating 3D AR pin with walking distance display

* 200m to 1km: On-screen directional compass guide

* Over 1km: Map fallback overlay with estimated walk time

#### Benefits:
* Instant visual identification of refuge points

* One-tap emergency contact desk routing

* Off-screen dynamic directional visual indicators

 ### 5. CIR-H – Community Incident Reporting & Heatmaps
#### Crowdsourced Threat Verification Platform

A dual-verification reporting pipeline converting user feedback and geotagged incident logs into live spatial risk heatmaps.

#### How It Works:
```
Plaintext
User Incident Snap -> Metadata Check -> AI Image Verification -> Grid Heatmap Mapping -> Public Warning Push
```
#### Benefits:
* EXIF and spatial verification prevents false reporting

* Automatic privacy blurring of faces before public upload

* Real-time geofenced community warning notifications


 ### Technology Stack
#### Mobile & AR Client
```
Plaintext
Unity (AR Foundation / ARCore / ARKit) • C# • Flutter (Companion App)
```
#### Backend & Infrastructure
```
Plaintext
Node.js / Python FastAPI • WebSockets • Redis • PostGIS
```
#### Computer Vision & AI
```
Plaintext
YOLOv8 • OpenCV • TensorFlow Lite • PyTorch
```
#### Database
```
Plaintext
MongoDB • PostgreSQL (Geospatial Spatial Indexes)
```
#### Getting Started
##### Prerequisites
```
Bash
Unity Hub >= 2022.3 LTS
Node.js >= 18.x
Python >= 3.9
Android Studio (ARCore) / Xcode (ARKit)
```
#### Installation
### 1️⃣ Clone Repository
```
Bash
git clone [https://github.com/harshkumar2112/SurakshaAR.git](https://github.com/harshkumar2112/SurakshaAR.git)
cd SurakshaAR
```
### 2️⃣ Backend Setup
```
Bash
cd backend
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
cp .env.example .env
python main.py
```
### 3️⃣ Unity / Mobile Setup
1. Open Unity Hub and add the project from src/SurakshaAR.

2. Ensure AR Foundation is active in Package Manager.

3. Select your target platform (Android/iOS) and build to an AR-supported device.

### API Endpoints
#### Navigation & Spatial Scoring
* POST /api/v1/route/safe-path - Fetch spatial route optimized for safety

* GET /api/v1/heatmap/spatial-grid - Retrieve regional threat index map

#### Emergency & Dispatch
* POST /api/v1/sos/trigger - Dispatch emergency payload with 3D anchors

* GET /api/v1/safe-havens/nearby - Fetch geofenced safe refuge zones

#### System Strengths
##### Technical Excellence
* Low-Latency AR - Sub-second visual world-space rendering

* Spatial Accuracy - Multi-sensor fusion using GPS, IMU, and visual odometry

* Edge AI - Local hazard detection running on-device via TFLite

##### Operational Benefits
* Zero Ambiguity - Direct visual arrows eliminate navigation stress

* Automated Dispatch - Sub-minute alert transmission times

* High Reliability - Offline fallback mechanism queues alerts during connection drops

### 🙏 Acknowledgments
* OpenCV and Ultralytics YOLO communities for vision algorithms

* Unity AR Foundation team for cross-platform AR tools

* OpenStreetMap contributors for geospatial mapping data
  
