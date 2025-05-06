# ✈️ Flight Delay Prediction

**A Deep Learning Model to Predict Flight Arrival Delays Using Travel Data**

---

## 🚀 Overview

This project uses a **neural network model** to predict whether a flight will be delayed and estimate the delay in minutes based on key features such as air time and distance. It includes data visualization, correlation analysis, model training, and real-time prediction capability.

Built with **TensorFlow (Keras)** and visualized using **Plotly**, **Matplotlib**, and **Seaborn**, this project is ideal for analyzing delay trends and making intelligent flight predictions.

---

## ✨ Features

* 🧠 Predicts **delay status** (on-time/delayed) and **delay duration**
* 📈 Visual insights: delay by airport, destination, and month
* 🔎 Correlation heatmap for numerical features
* 💻 Scaled data using **StandardScaler**
* 🏃‍♀️ Real-time user input for custom flight delay prediction
* 📊 Bar graphs built using **Plotly Express**

---

## 🛠️ Tech Stack

* **Language**: Python
* **Libraries**:

  * Pandas, NumPy (Data Handling)
  * Matplotlib, Seaborn, Plotly (Visualization)
  * Scikit-learn (Preprocessing, Split, Scaling)
  * TensorFlow / Keras (Deep Learning)

---

## 📁 Dataset

* `flight_delay_predict.csv` – contains flight-level features:

  * `AirTime` – Actual air time of the flight
  * `Distance` – Distance traveled
  * `FlightDate`, `Origin`, `Dest` – For delay trends and visualizations
  * `ArrDelayMinutes`, `is_delay` – Target values

---

## 🧠 Model Architecture

* **Input Layer**: 2 features – `AirTime` and `Distance`
* **Hidden Layers**:

  * Dense(64) with ReLU + Dropout(0.5)
  * Dense(32) with ReLU + Dropout(0.5)
* **Output Layer**: Dense(2) – Predicts `ArrDelayMinutes` and `is_delay` (0 or 1)

---

## 📊 Visualizations

* 📍 Average Delay by Origin Airport
* 🛬 Average Delay by Destination
* 📅 Delay Trends by Month
* 🔥 Correlation Heatmap of Numerical Features

---

## ▶️ How to Use

### 1. Train the Model

```bash
python your_script.py
```

### 2. Make Real-Time Predictions

When prompted, enter:

* `Air Time` in minutes
* `Distance` in miles

The model will return:

* Estimated delay in minutes
* Whether the flight is likely **delayed or not**

---

## 📦 Output Example

```bash
Enter Air Time in minutes: 145
Enter Distance in miles: 1200
The flight is delayed by 23.42 minutes.
```

---

## 💾 Saved Model

The trained model is saved in `.keras` format:

```
/content/my_model.keras
```

---
