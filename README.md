# Soil-Perameter-Prediction
This internship project at NECTAR involved real-time monitoring and predicting soil parameters like moisture, temperature, and electrical conductivity. It utilised microcontrollers for sensor data acquisition and incorporated data preprocessing for a machine learning model, with applications in precision agriculture and sustainable farming.

# 🌾 IoT-Based Soil Parameter Prediction System

A smart agriculture project that uses sensors to collect real-time soil data (moisture, temperature, EC, and light) and predicts optimal growing conditions using machine learning.

---

## 📌 Features

- 🌱 Real-time monitoring of key soil parameters  
- 🔗 IoT integration using **ESP32/Arduino + Sensors**  
- 📊 Local or cloud-based data logging  
- 🤖 Predictive analysis using **machine learning models**  
- 📉 Calibration & accuracy tuning for real-world deployment  

---

## 🧪 Parameters Measured

- 🌡️ **Soil Temperature**  
- 💧 **Soil Moisture**  
- ⚡ **Soil Electrical Conductivity (EC)**  
- ☀️ **Ambient Light Intensity**

---

## 🔧 Hardware Components

- LoRaWAN Gateway  
- Soil Moisture Sensor  
- DHT11/DHT22 (for temperature)  
- TDS/EC Sensor  
- LDR or BH1750 (for light)  

---

## 💻 Software Stack

- **Languages:** Python  
- **ML Libraries:** Pandas, Scikit-learn, NumPy, Matplotlib  
- **Tools:** Google Colab 
- **Protocols:** UART/I2C (for sensor communication)

---

## 📁 Folder Structure
iot-soil-parameter-prediction/
- ├── dataset/
- │     └── soil_data.csv
- ├── ml_model/
- │     └── soil_perameter_prediction.py
- └── README.md

---

## 🧠 Model Details

- **Algorithm**: Linear Regression (for baseline prediction)
- **MSE**: `0.569`
- **RMSE**: `0.754`
- **R² Score**: `NaN` (due to zero variance in target during test)

> ⚠️ *R² being NaN indicates the target values in the test set may be constant. Review dataset for variance.*

---

## 🚀 How to Use

1. **Connect sensors** to ESP32 or Arduino Uno
2. Upload the code from `hardware/Arduino_Code.ino`
3. Log the data via Serial Monitor or save to `.csv`
4. Run `train_model.py` to train the regression model
5. Predict new values with `predict.py`

---

## 📊 Sample Output

```bash
MSE of Linear Regression:  0.569
RMSE of Linear Regression:  0.754
R² of Linear Regression:  nan
```

---
## ✅ To-Do
- Collect and clean soil data
- Train baseline model
- Add cloud data logging (Firebase / ThingSpeak)
- Integrate GUI for real-time visualization

---

## 👨‍💻 Author
Pankaj Saraswat
B.Tech, Electronics & Communication
NIT Meghalaya
📧 Email: pksdoom@gmail.com


