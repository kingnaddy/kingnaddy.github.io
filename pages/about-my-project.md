---
layout: project
title: About My Project
permalink: /about-my-project.html

subtitle: Campus Sustainability & Intelligent Resource Management
project_title: "Smart AI-Based Waste Bin Monitoring and Collection Optimization on Morgan State University Campus"

problem: |
   Inefficient waste collection on campus leads to overflowing bins, sanitation issues, and unnecessary operational costs. There is currently no adaptive system that can monitor bin fill levels in real time and optimize collection routes to ensure timely service and campus cleanliness.

approach: |
  This project implements a three-part AI pipeline:
  
  1. **Computer Vision Monitoring**  
     – Deploy IoT cameras at strategic bins and train a YOLO object-detection model to estimate fill levels from images.  
  2. **Predictive Forecasting**  
     – Aggregate time-series data on bin usage and train an LSTM network to forecast future overflow probabilities.  
  3. **Route Optimization**  
     – Use reinforcement learning (e.g. PPO or DQN) to develop an agent that dynamically schedules collection routes and frequencies based on current and predicted fill levels.
  
  Prototype development will leverage Python (Ultralytics YOLOv5, TensorFlow/Keras, PyTorch), AWS EC2 or Google Colab Pro+, and ROS for simulation of robotic collection vehicles.

outcome: |
  By the end of the 10-week program, the team will deliver:
  
  - A trained YOLO model capable of real-time bin fill detection (mAP ≥ 0.75).  
  - An LSTM forecasting module with RMSE ≤ 10% on hold-out waste accumulation data.  
  - A reinforcement learning prototype demonstrating optimized collection routes with measurable reward convergence.  
  - An interactive dashboard visualizing bin statuses, forecasts, and recommended collection plans.  
  - Technical documentation and a symposium poster detailing system architecture, model performance metrics, and sustainability impact.

final_report_url: https://dl.icdst.org/pdfs/files/22e390b2eb0c8e951f3a742fda5b2d1d.pdf

grad_mentor:
  name: Oluwafemi Ifesanmi
  email: olife2@morgan.edu

faculty_mentor:
  name: Dr. Steve Efe
  email: steve.efe@morgan.edu
---
