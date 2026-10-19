# 📈 Numerical Integration Methods: Trapezoidal & Simpson's Rules

[![Jupyter Notebook](https://shields.io)](https://jupyter.org)
[![Python](https://shields.io)](https://python.org)
[![License: MIT](https://shields.io)](https://opensource.org)

A comprehensive **Jupyter Notebook** implementation demonstrating the power of numerical integration. This repository explores how to efficiently approximate the **Area Under the Curve (AUC)** for definite integrals using classic mathematical algorithms.

---

## 🚀 Key Methods Implemented

### 📐 1. The Trapezoidal Rule
* **The Concept:** Unlike standard Riemann sums that use rigid rectangles, this rule divides the total interval into **\(n\) sub-intervals (trapezoids)** of uniform width. 
* **The Mechanics:** It calculates the area of each trapezoid using standard geometric formulas and sums them up.
* **Assumption:** The top edge of each sub-interval is assumed to be a **straight linear line**.

### 🎢 2. Simpson's Rule
* **The Concept:** Takes approximation a step further by replacing straight lines with **parabolic arcs (quadratic curves)** across the sub-intervals (\(n\)).
* **The Mechanics:** By fitting second-degree polynomials to the data points, it naturally minimizes error margins.
* **Assumption:** The top boundary of each segment follows a **smooth curve**, yielding significantly higher accuracy than linear methods.

---

## 📊 Quick Method Comparison

| Feature | Riemann Sums | Trapezoidal Rule | Simpson's Rule |
| :--- | :--- | :--- | :--- |
| **Top Boundary** | Flat / Constant (\(x^0\)) | Linear / Straight (\(x^1\)) | Parabolic / Quadratic (\(x^2\)) |
| **Geometry Used** | Rectangles | Trapezoids | Parabolic Segments |
| **Relative Accuracy**| 🔴 Low | 🟡 Moderate | 🟢 High |
| **Best Used For** | Basic Concept Teaching | Linear Data Trends | Smooth, Curving Datasets |

---

## ⚙️ Real-World Applications

Numerical integration acts as a foundational tool across multiple industries where exact algebraic solutions are impossible to find:
* **Physics & Engineering:** Estimating total displacement from variable velocity data, or calculating total mechanical work done from raw experimental sensor outputs.
* **Finance:** Approximating the present value of fluctuating, continuous cash flow stream totals.
* **Data Science:** Calculating the Area Under the ROC Curve (AUC-ROC) to benchmark machine learning model performance.

---

## 🛠️ Getting Started

### Prerequisites
Make sure you have Python and the following libraries installed:
```bash
pip install numpy matplotlib jupyter
```

### Running the Notebook
1. Clone this repository:
   ```bash
   git clone https://github.com
   ```
2. Navigate into the project folder:
   ```bash
   cd YOUR_REPOSITORY_NAME
   ```
3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Open the main `.ipynb` file to run the integration simulations!

---

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
