# 📱 Termux Memory Engine: Hybrid Lenovo Legion Tab Price Tracker

A resilient, mobile-optimized context-tracking application built entirely inside **Android Termux** for **The Hangover Part AI Hackathon**.

This engine features two distinct development pipelines built to track retail price shifts for the **Lenovo Legion Tab (8.8 inch Gen 2)** across Lenovo India and Amazon.

## 🚀 Dual-Track Architecture Blueprint

### 🖥️ 1. Open Source Build (Targeting MacBook Neo Track)
- **File**: `os_tracker.py`
- **Engine**: Emulates Cognee's open-source SQLite/Local data engine framework. 
- **Resilience**: Features a localized graph fallback tier to bypass native mobile compilation bottlenecks (`lancedb`) and serve query responses offline.

### 📱 2. Cloud Platform Build (Targeting iPhone 17 Track)
- **File**: `tracker.py`
- **Engine**: Fully mapped to hook into Cognee's restored Cloud Gateway infrastructure.
- **Resilience**: Captures API network status warnings cleanly to guarantee data updates without experiencing AI amnesia.

## 📊 Retained Graph Context
- **Lenovo India Store**: ₹39,999 Base Rate
- **Amazon Import Listings**: ₹42,500 Market Rate
- **Hardware Profile**: Snapdragon 8+ Gen 1, 12GB RAM, 256GB Storage, 144Hz Display.

## 💻 Local CLI Execution
Ensure dependencies are installed in Termux, then launch either framework:
```bash
pip install requests
python os_tracker.py  # Run the Open Source Build
python tracker.py     # Run the Cloud Build
```
