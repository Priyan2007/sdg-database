# 🌍 SDG Progress Graph (Python Matplotlib Project)

## 📌 Project Description

The **SDG Progress Graph** is a simple Python project that visualizes data related to different **Sustainable Development Goals (SDGs)** using a bar chart.

This project is inspired by the global goals introduced by the United Nations to promote sustainable development.

The program uses the `matplotlib` library to create a graphical representation of progress or scores for selected SDGs.

---

## 🎯 Features

* 📊 Displays SDG data using a bar graph
* 🖥️ Simple and easy-to-understand visualization
* 🧾 Uses predefined dataset
* 🎨 Clean and readable graph layout

---

## 🛠️ Technologies Used

* Python 3.x
* Matplotlib (`matplotlib.pyplot`)

---

## 📂 SDG Categories Used

The following SDGs are included in this project:

* No Poverty
* Quality Education
* Climate Action
* Good Health
* Clean Energy

---

## 📊 Data Representation

Each SDG is assigned a score representing its progress level:

| SDG Goal          | Score |
| ----------------- | ----- |
| No Poverty        | 80    |
| Quality Education | 85    |
| Climate Action    | 75    |
| Good Health       | 82    |
| Clean Energy      | 88    |

---

## ▶️ How to Run

1. Install Python (3.x)
2. Install matplotlib (if not installed):

```bash
pip install matplotlib
```

3. Save the code as `sdg_graph.py`
4. Run the program:

```bash
python sdg_graph.py
```

---

## 🖼️ Output

* A bar graph window will open displaying SDG scores
* Each bar represents the progress of a specific SDG
* X-axis shows SDG categories
* Y-axis shows corresponding scores

---

## 📚 Concepts Used

* Data visualization
* Bar chart plotting
* Labeling and formatting graphs
* Python lists

---

## 🚀 Future Enhancements

* 📊 Add dynamic user input
* 📈 Use real-world SDG datasets
* 🎨 Customize graph colors and styles
* 🔄 Convert to GUI-based application

---
## Program
```
import matplotlib.pyplot as plt

# SDG categories (minimum 5)
sdg_goals = [
    "No Poverty",
    "Quality Education",
    "Climate Action",
    "Good Health",
    "Clean Energy"
]

# Corresponding scores/data
scores = [80, 85, 75, 82, 88]

# Create bar graph
plt.bar(sdg_goals, scores)

# Labels and title
plt.xlabel("SDG Goals")
plt.ylabel("Score")
plt.title("SDG Progress Graph")

# Rotate labels (important for clarity)
plt.xticks(rotation=30)

# Show graph
plt.show()
```
## Output

<img width="832" height="701" alt="image" src="https://github.com/user-attachments/assets/a2582ff8-e694-46e6-b330-af73e76329ea" />

# SDG categories (minimum 5)
sdg_goals = [
    "No Poverty",
    "Quality Education",
    "Climate Action",
    "Good Health",
    "Clean Energy"
]

# Corresponding scores/data
scores = [80, 85, 75, 82, 88]

# Create bar graph
plt.bar(sdg_goals, scores)

# Labels and title
plt.xlabel("SDG Goals")
plt.ylabel("Score")
plt.title("SDG Progress Graph")

# Rotate labels (important for clarity)
plt.xticks(rotation=30)

# Show graph
plt.show()

## ✅ Result

Thus, the **SDG Progress Graph** is successfully implemented using Python and matplotlib to visualize SDG data effectively.

