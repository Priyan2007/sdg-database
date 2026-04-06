# **SDG-13 Climate Analysis and Prediction System for Tamil Nadu**

---

## 🎯 **Aim**

To analyze temperature rise and rainfall patterns in Tamil Nadu using Python (without external dataset) and to predict future climate conditions supporting **SDG 13 – Climate Action**.

---

## 🎯 **Objectives**

* To study climate trends using predefined data
* To visualize temperature and rainfall using graphs
* To predict future values using machine learning
* To identify extreme climate conditions

---

## 🧰 **Requirements**

* Python 3.x
* Libraries: Pandas, Matplotlib, NumPy, Scikit-learn

---

## 📊 **Theory**

Climate change is causing rising temperatures and irregular rainfall in Tamil Nadu. The state depends heavily on the **northeast monsoon**, making it vulnerable to droughts and floods.

This project uses:

* **Pandas** for handling data
* **Matplotlib** for plotting graphs
* **Linear Regression** for predicting future values

Instead of using an external CSV file, the dataset is created directly within the Python program.

---

## ⚙️ **Procedure**

1. **Create Data**
   Define temperature and rainfall data inside the program.

2. **Convert to DataFrame**
   Use Pandas to convert the data into tabular form.

3. **Plot Graphs**

   * Plot temperature vs year
   * Plot rainfall vs year

4. **Build Prediction Model**
   Use Linear Regression to predict:

   * Future temperature
   * Future rainfall

5. **Display Results**
   Show graphs and predicted values on screen.

6. **Generate Alerts**

   * Heatwave alert if temperature is high
   * Drought alert if rainfall is low
   * Flood alert if rainfall is high

---

## 💻 **Program**

```python
import pandas as pd
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression
import numpy as np

data = {
    'Year': [2022, 2023, 2024, 2025],
    'Avg_Temperature': [34.5, 35.2, 36.1, 36.8],
    'Rainfall': [950, 870, 920, 880]
}

df = pd.DataFrame(data)

plt.figure()
plt.plot(df['Year'], df['Avg_Temperature'], marker='o')
plt.title("Temperature Trend")
plt.xlabel("Year")
plt.ylabel("Temperature (°C)")
plt.show()

plt.figure()
plt.plot(df['Year'], df['Rainfall'], marker='o')
plt.title("Rainfall Trend")
plt.xlabel("Year")
plt.ylabel("Rainfall (mm)")
plt.show()

X = df[['Year']]

model = LinearRegression()
model.fit(X, df['Avg_Temperature'])
pred_temp = model.predict([[2026]])

model.fit(X, df['Rainfall'])
pred_rain = model.predict([[2026]])

print("Predicted Temperature:", pred_temp[0])
print("Predicted Rainfall:", pred_rain[0])
```

## OUTPUT
<img width="877" height="727" alt="image" src="https://github.com/user-attachments/assets/ff0d02db-165c-424d-b4ca-d57ce22c68c4" />


## 📈 **Result**

* The temperature graph shows a **steady increase**, indicating rising heat levels.
* The rainfall graph shows **irregular variation**, indicating unstable monsoon patterns.
* Predicted Temperature for 2026 is approximately **37°C**.
* Predicted Rainfall for 2026 is approximately **860 mm**.

---

## 📌 **Conclusion**

The project successfully analyzes climate trends and predicts future conditions using Python without relying on external data files. It helps in understanding climate change impacts and supports **sustainable planning under SDG 13 (Climate Action)**.

---

## 🚀 **Future Enhancements**

* Use real-time datasets
* Add GUI interface
* Extend prediction for multiple years
* Integrate live weather APIs

---
