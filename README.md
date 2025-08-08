# Aindo Hackathon 2024 - Winner Solution 🏆

**Indoor Human Movement Prediction using IoT Sensors**

---

## Overview

Winner solution for the **Aindo Hackathon 2024**. The challenge was to predict human movement within a house across 5 rooms (Living Room, Bedroom, Bathroom, Kitchen, Hallway) using IoT sensor data.

## Problem

**Input Data:**
- Motion sensors (binary 0/1) for each room
- Environmental sensors: temperature, humidity, CO2, gas sensors (MOX1-4), CO levels
- Temporal information (timestamps)

**Goal:** Predict person's location at each timestamp

## Solution

**Our Winning Approach:**
- **Random Forest** models for robust feature analysis
- **LSTM networks** for temporal sequence modeling
- **Advanced feature engineering** with variance-based environmental features
- **Data preprocessing** pipeline for sensor noise reduction

## Key Files

- `LSTM_final.ipynb` - LSTM implementation with PyTorch Lightning
- `grafici.ipynb` - Data analysis and visualization
- `data/clean_data.csv` - Preprocessed training data (265K samples)
- `results/BinaryBrilliance.csv` - Final predictions

## Results

🥇 **1st Place** - Team "Binary Brilliance"

Our combination of traditional machine learning (Random Forest) and deep learning (LSTM) achieved the best performance on the test dataset by effectively capturing both spatial relationships and temporal movement patterns.

## Usage

```bash
# Install dependencies
pip install torch pytorch-lightning pandas numpy scikit-learn matplotlib

# Run LSTM model
jupyter notebook LSTM_final.ipynb

# View data analysis
jupyter notebook grafici.ipynb
```

---

**Technologies:** Python, PyTorch, Random Forest, LSTM, IoT Sensors, Time Series Prediction