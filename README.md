# nasa-turbofan-RUL
# Predictive Maintenance using CNN-LSTM for RUL Prediction

## Overview

This project focuses on predicting the **Remaining Useful Life (RUL)** of turbofan engines using sensor data.

The goal is to build a system that can estimate how long an engine will continue to operate before failure by learning degradation patterns over time.

---

##  Dataset

NASA C-MAPSS Dataset (FD004)

* Multiple operating conditions
* Multiple fault modes
* Simulates real-world engine degradation

---

##  Approach

### Data Processing

* Created target variable (RUL = remaining life cycles)
* Removed low-variance features
* Applied normalization (per engine for deep learning)
* Generated time-series sequences

---

###  Models Used

* Random Forest (baseline)
* Gradient Boosting
* LSTM (time-series model)
* CNN + Bidirectional LSTM (**final model**)

---

## Results

| Model             | RMSE     |
| ----------------- | -------- |
| Random Forest     | XX       |
| Gradient Boosting | XX       |
| LSTM              | XX       |
| CNN + BiLSTM      | **Best** |

---

## 🔍 Key Insights

* Engine degradation is gradual and follows observable patterns
* Certain sensors have strong correlation with failure
* Deep learning models outperform traditional ML due to temporal modeling
* Prediction becomes more difficult under multiple operating conditions (FD004)

---

## Visualizations

* Sensor degradation trends
* Correlation heatmap
* Interactive 3D plots
* Model comparison charts

---

## Conclusion

This project demonstrates that machine learning and deep learning techniques can effectively predict engine failure before it occurs.

The hybrid CNN + LSTM model performs best as it captures both:

* local sensor patterns (CNN)
* temporal dependencies (LSTM)

Such systems are useful in predictive maintenance to reduce failures, optimize costs, and improve safety.

---

##  Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* TensorFlow / Keras
* Matplotlib, Seaborn
* Plotly

---

##  Future Work

* Attention-based models
* Transformer architectures
* Real-time deployment systems

---

##  Author

SHAH NASHIT
