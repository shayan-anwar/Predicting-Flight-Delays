# Predicting-Flight-Delays
## 📌 Overview

Flight delays can significantly impact airline operations and passenger satisfaction. This project investigates the feasibility of predicting arrival and departure delays in advance using historical data and supervised learning techniques.

---

## 🧠 Problem Statement

**Can we accurately predict flight delay times based on flight schedule and historical delay data?**

---

## 📂 Dataset

- **Source:** [Kaggle - Predicting Flight Delay](https://www.kaggle.com/code/bobirino/predicting-flight-delay/notebook)
- **Year:** 2016
- **Key Features (29 Total):**
  - Flight Date (Year, Month, Day, DayOfWeek)
  - Scheduled & Actual Departure/Arrival Times
  - Delay Times: Arrival, Departure, Carrier, Weather, NAS, Security, Late Aircraft
  - Distance, Taxi Time, Elapsed Time
  - Cancellation & Diversion Status
  - Airline Information (Carrier Code, Flight Number, Tail Number)

---

## 🔍 Exploratory Data Analysis & Visualization

- 📊 Delay distribution by **Day of Week** and **Day of Month**
- ✈️ Comparisons of **Actual vs Scheduled** times
- 📈 Carrier delay reasons & performance analysis
- 🔍 Patterns in delay propagation (e.g., late aircraft effects)

---

## 🏗️ Feature Engineering

- Created meaningful features like:
  - `DelayDifference` (ArrDelay - DepDelay)
  - `TotalElapsedTime`
  - `IsWeekend`, `IsMorningFlight`, etc.
- Handled null values and encoded categorical variables
- Normalized features for better model compatibility

---

## 🤖 Model Development

We trained and evaluated several regression models:

### ✅ Linear Regression
- Assumes linear relationships between features and delay
- Fast and interpretable

### 🌲 Random Forest Regression
- Captures non-linear patterns and interactions
- Reduces variance through ensemble averaging

### 🔥 Gradient Boosting Regression
- Builds strong learners sequentially
- Performs well on noisy, non-linear datasets

---

## 📈 Evaluation Metric

- **Mean Squared Error (MSE)** was used to evaluate model performance.
