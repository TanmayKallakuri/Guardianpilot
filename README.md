# GuardianPilot ✈️

> **Preventing spatial disorientation accidents through real-time situational awareness monitoring**

[![Built for Navi AI Hackathon](https://img.shields.io/badge/Navi%20AI-Hackathon%202025-blue)](https://navi.ai)
[![Powered by You.com](https://img.shields.io/badge/Powered%20by-You.com-orange)](https://you.com)
[![Google Maps](https://img.shields.io/badge/Google-Maps%20API-green)](https://maps.google.com)

## 🎯 Problem Statement

**40% of general aviation fatal accidents** are caused by spatial disorientation and loss of situational awareness. Traditional warning systems only alert when parameters exceed thresholds—often **too late for recovery**.

GuardianPilot detects **degrading situational awareness patterns** before they become critical, providing pilots with precious seconds to recover.

---

## 🚀 Key Features

### 1. **SA Score Algorithm (0-100)**
Real-time situational awareness metric that quantifies pilot awareness based on flight telemetry patterns.

- **100** = Perfect situational awareness
- **70-85** = Caution (minor degradation)
- **50-70** = Warning (significant degradation)
- **<50** = Critical (immediate action required)

### 2. **Pattern-Based Detection**
Detects four critical SA loss patterns:

| Pattern | Description | NTSB Relevance |
|---------|-------------|----------------|
| 🌀 **Graveyard Spiral** | Increasing bank + descent (spatial disorientation) | 40% of fatal GA accidents |
| ⛰️ **Altitude Unawareness** | Descending into terrain without correction | CFIT accidents |
| 🔄 **Disoriented Maneuvering** | Erratic inputs indicating pilot behind aircraft | Loss of control |
| ⚡ **Energy Mismanagement** | Approaching stall or overspeed | Stall/spin accidents |

### 3. **You.com Integration** 🔍
- Real-time NTSB incident database search
- Historical context for each detected pattern
- Lessons learned from similar accidents
- Powered by You.com Search API

### 4. **Google Maps Visualization** 🗺️
- Interactive terrain-aware flight path visualization
- Detection markers with urgency color-coding
- Toggle between terrain and satellite views
- Measure distances and analyze spatial relationships

### 5. **Impact Analysis**
Quantifies system effectiveness with before/after comparison:

| Scenario | Warnings Provided | Lead Time |
|----------|-------------------|-----------|
| **Without GuardianPilot** | 0 | 0 seconds |
| **With GuardianPilot** | ✅ Pattern-based alerts | **18+ seconds** early warning |

---

---

## 🛠️ Technology Stack

- **Frontend:** Streamlit
- **Visualization:** Plotly, Folium (Google Maps integration)
- **Data Processing:** Pandas, NumPy
- **Pattern Detection:** Custom algorithms based on NTSB accident analysis
- **APIs:**
  - You.com Search API (incident context)
  - Google Maps (terrain visualization)

---

## 📦 Installation

### Prerequisites
- Python 3.8+
- pip

### Setup
```bash
