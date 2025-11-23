# 🚦 Smart City Traffic Management System

![Team](https://img.shields.io/badge/Team-Witty%20Hackers-blueviolet)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![Stack](https://img.shields.io/badge/Stack-MERN%20%2B%20Python%20ML-orange)

**Team:** Witty Hackers  
**Members:** * Shaldon Barnes (NNM23CS172)
* Anish Bhat (NNM23CS036)

---

## 📘 Overview

The **Smart City Traffic Management System** is an AI-driven initiative designed to transform urban mobility.  
By combining adaptive signal control, real-time monitoring, and predictive analytics, our system aims to **reduce congestion, optimize travel time**, and **minimize CO₂ emissions** in cities.

---

## 🚧 The Problem – Urban Traffic Congestion

Urban commuters spend **over 100 hours per year** stuck in traffic, wasting time, fuel, and energy.  
Traditional traffic systems rely on static timers that cannot adapt to changing road conditions, leading to:
* Longer waiting times
* Inefficient traffic flow
* Increased CO₂ emissions and air pollution

This calls for a **dynamic, intelligent solution** that adapts in real-time.

---

## 💡 Our Solution – Intelligent, Proactive System

Our system introduces a smart, AI-based framework that **monitors live traffic**, **adapts signal timing**, and **predicts congestion** before it occurs.

**Core Features:**
1.  **Adaptive Signal Control:** Adjusts green/red durations dynamically based on live traffic density.
2.  **Predictive Analytics:** Uses machine learning (Random Forest / LSTM) to forecast congestion 15–30 minutes ahead.
3.  **Real-Time Monitoring Dashboard:** Displays live traffic heatmaps and junction-level insights.
4.  **Proactive Management:** Enables authorities to make data-driven, preemptive decisions.

---

## 🧩 System Architecture

**Data Flow:**
* **Traffic Data Source:** Real-time feeds (Google Maps, OpenStreetMap) or simulated CSV datasets.
* **AI/ML Module:** Predicts congestion patterns using live and historical data.
* **Backend (Node.js + Express):** Implements adaptive signal logic and provides REST APIs.
* **Database:** PostgreSQL (structured logs) and MongoDB (historical predictions).
* **Traffic Signal Hardware:** Receives dynamic timing updates.

---

## 🧠 Technology Stack

| Layer | Technology |
| :--- | :--- |
| **Backend** | Node.js, Express |
| **AI/ML Models** | Random Forest, LSTM (scikit-learn, TensorFlow) |
| **Databases** | PostgreSQL |
| **Integration** | REST APIs for real-time data and emergency vehicle events |

---

## 📊 Real-Time Monitoring Dashboard

The dashboard empowers traffic operators with live visual insights:
* **Dynamic heatmaps** showing congestion severity (Green → Clear, Yellow → Moderate, Red → Heavy).
* **Junction-level analytics:** Vehicle count, average waiting time, and signal status.
* **Predictive overlays** showing congestion hotspots up to 30 minutes ahead.

---

## 🤖 AI-Driven Optimization

Our adaptive algorithm distributes green light durations proportional to traffic volume, optimizing flow across intersections.  
Machine learning models forecast congestion trends based on:
* Time of day
* Live data inputs
* Historical patterns

This allows **preemptive traffic control** and reduces gridlocks significantly.

---

## 🌍 Tangible Benefits

| Stakeholder | Benefit |
| :--- | :--- |
| **City Authorities** | Move from reactive to proactive management, improve emergency response. |
| **Commuters** | 20–30% reduction in average travel time, enhanced productivity. |
| **Environment** | Lower fuel waste and reduced CO₂ emissions. |

---

## 🏆 Hackathon Context

Developed as part of an **Aceathon challenge**, this project demonstrates how **AI + IoT + Data Analytics** can power the next generation of **Smart City traffic ecosystems**.

---

## 📂 Repository Structure

```text
SMART_TRAFFIC_MANAGEMENT_SYSTEM/
│
├── backend/                       # Node.js + Express backend
│   ├── node_modules/
│   ├── src/
│   │   ├── routes/
│   │   │   └── trafficRoutes.js
│   │   ├── controllers/
│   │   │   └── trafficController.js
│   │   ├── models/
│   │   │   └── logsModel.js
│   │   ├── services/
│   │   │   └── signalOptimizer.js
│   │   └── app.js
│   ├── .env
│   ├── package.json
│   ├── package-lock.json
│   └── README.md
│
├── frontend/                      # React + Vite Frontend
│   ├── node_modules/
│   ├── public/
│   │   └── index.html
│   ├── src/
│   │   ├── components/
│   │   │   ├── Heatmap.jsx
│   │   │   └── TrafficCard.jsx
│   │   ├── pages/
│   │   │   └── Dashboard.jsx
│   │   ├── styles/
│   │   │   └── dashboard.css
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── package.json
│   ├── package-lock.json
│   ├── vite.config.js
│   ├── tsconfig.json
│   └── README.md
│
├── ml/                            # Machine Learning module
│   ├── __pycache__/
│   ├── data/
│   │   └── traffic_data.csv
│   ├── models/
│   │   ├── traffic_model.joblib
│   │   └── lstm_model.h5
│   ├── scripts/
│   │   ├── train_model.py
│   │   ├── predictor.py
│   │   └── vision_counter.py
│   ├── utils/
│   │   └── csv_generator.py
│   ├── myenv/                     # Python virtual environment
│   ├── requirements.txt
│   └── README.md
│
├── docs/                          # Documentation
│   ├── architecture_diagram.png
│   └── system_design.md
│
├── .gitignore
├── README.md                      # Main project description
└── LICENSE