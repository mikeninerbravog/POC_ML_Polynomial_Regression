# Machine Learning - Polynomial Regression Proof of Concept (POC)

This repository demonstrates how **Polynomial Regression** improves predictions when data follows a non-linear trend. The examples focus on two real-world scenarios:

1. **Predicting Plant Growth**: Estimating a plant’s height over time, considering that growth starts slow, accelerates, and later stabilizes.
2. **Predicting a Car’s Speed Over Time**: Modeling a car’s acceleration, showing that speed increases rapidly at first but eventually stabilizes.

## What is Polynomial Regression?

**Polynomial Regression** is an extension of **Linear Regression** that fits a **curved line** instead of a straight one. It is useful when relationships between variables are not simply increasing or decreasing but follow a **non-linear pattern**.

### Why Use Polynomial Regression?
- **Captures complex relationships**: Unlike linear regression, it can model data with peaks and valleys.
- **Better fit for real-world scenarios**: Many natural and mechanical processes do not follow a straight-line trend.
- **Used in various fields**: Applications range from **biology** to **engineering** and **AI**.

## Running on Google Colab

### Step 1: Open the Notebooks in Colab
Click the links below to open the examples directly in **Google Colab**:
- [Predicting Plant Growth](https://colab.research.google.com/github/mikeninerbravog/POC_ML_Polynomial_Regression/blob/master/POC_ML_PolynomialRegression.ipynb)
- [Predicting a Car’s Speed Over Time](https://colab.research.google.com/github/mikeninerbravog/POC_ML_Polynomial_Regression/blob/master/POC_ML_PolynomialRegression.ipynb)

### Step 2: Install Dependencies (if needed)
Google Colab usually has all required libraries pre-installed. If needed, run:
```python
!pip install numpy matplotlib scikit-learn
```

### Step 3: Run the Cells
Each notebook contains explanations, data, and visualizations. Simply **execute the cells** in order.

---

## Example 1: Predicting Plant Growth 🌱

This model predicts how a **plant's height** changes over time. Instead of a **straight-line prediction** (Linear Regression), **Polynomial Regression** captures how the growth rate varies.

- **Input Features**:
  - Days of observation
- **Output**: Predicted plant height
- **Comparison**: Standard Linear Regression vs. Polynomial Regression (Degree 2)

### Notebook Highlights:
- **Linear Regression** attempts to fit a straight line, leading to poor predictions.
- **Polynomial Regression** (degree 2) creates a **curved** trend line that better matches plant growth.
- A **scatter plot** visualizes real vs. predicted values.

---

## Example 2: Predicting a Car’s Speed Over Time 🚗

This model predicts how a **car’s speed** changes over time during acceleration. Since the speed does not increase at a constant rate, a **Polynomial Regression model** is needed.

- **Input Features**:
  - Time (seconds)
- **Output**: Predicted car speed (km/h)
- **Comparison**: Standard Linear Regression vs. Polynomial Regression (Degree 2)

### Notebook Highlights:
- **Linear Regression** forces a straight-line prediction, failing to model acceleration and speed stabilization.
- **Polynomial Regression** captures the **initial acceleration and later speed stabilization**.
- The **Mean Squared Error (MSE)** is compared to evaluate model performance.

---

## Visualizing Results

Each notebook generates a **scatter plot** comparing **Linear Regression** and **Polynomial Regression**:
- **Blue dots**: Actual recorded data.
- **Red dashed line**: Linear Regression prediction.
- **Green line**: Polynomial Regression prediction (better fit).

---

## Conclusion

**Polynomial Regression** is a fundamental technique in Machine Learning for modeling **non-linear relationships**. It ensures better predictions in real-world scenarios, such as **biological growth patterns, vehicle dynamics, and many engineering applications**.

## License

This project is released under the MIT License.
