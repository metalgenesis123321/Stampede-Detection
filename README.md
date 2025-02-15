# Stampede-Detection-System

# Overview
This project aims to develop a stampede detection system that analyzes crowd density, changes in direction, and motion patterns to detect potential stampede risks. The system processes images from an online dataset using FiftyOne and YOLO, identifies anomalous movement, and triggers alerts in high-risk scenarios.

# Problem Statement
In dense environments such as metro stations, concerts, and public gatherings, there is a possibilty of crowd surge, that can lead to serious injuries or fatalities. The objective of this project is to:

- Detect crowd density levels to assess congestion risk.
- Identify anomalous movement patterns that indicate potential stampedes.
- Recognize falling individuals and provide real-time alerts when stampede risks are detected.

#  Implementation

# 1. Data Collection & Processing
  - Real-time Video Input: Surveillance cameras, drones
  - Preprocessing: Frame extraction, noise reduction, and stabilization.
  - We used FiftyOne library for frame extraction and labelling.
    
# 2. AI-based Crowd Analysis
   1. Crowd Density Analysis
      - Detect people per square meter using object detection (YOLO).
      - Predict trends using historical data and time-series analysis.
   
   2. Sudden Change in Direction
      - Optical Flow Analysis (Lucas-Kanade, Farneback) to track movement vectors.
      - Anomaly Detection: Identify rapid directional shifts.
      - Correlate with audio signals (if available) for external disturbances.
        
 3.	Motion Patterns & Erratic Behavior
      - Track acceleration spikes using trajectory analysis.
      - Identify unnatural clustering with density-based clustering (DBSCAN).        

# 3. Alert Mechanism & Visualization
  - Risk Flags: High & Critical levels based on predefined thresholds.
  - Live Dashboard: Real-time alerts, risk zones.
  - Automated Notifications: Alerts sent to security teams via SMS/IoT integration.

# Links to Dataset
- https://github.com/mchengny/RWF2000-Video-Database-for-Violence-Detection
- https://www.kaggle.com/datasets/danaelisanicolas/high-density-crowd-counting/data




