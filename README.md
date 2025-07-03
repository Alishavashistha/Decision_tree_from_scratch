# 📈 Simple Decision Tree Regressor (From Scratch)

This project demonstrates how to build a **Decision Tree Regressor** from scratch using Python and NumPy. It includes two models:
- A **1-split decision stump**, which splits the data at the best threshold once.
- A **full binary decision tree** built up to **depth 4**, using information gain to decide splits.

The project also visualizes the synthetic dataset and tree predictions using Matplotlib.

---

## 📁 Files Included

- `decision_tree_regressor.py`  
  Main script containing code to:
  - Generate synthetic data
  - Build the decision tree
  - Compute information gain
  - Visualize predictions

- `README.md`  
  This file.

---

## 🔧 How It Works

1. **Synthetic Data Generation**  
   Generates 100 samples using the equation:

   \[
   y = 4 + 3x + \text{noise}
   \]

2. **1-Split Decision Tree (Stump)**  
   - Finds the best threshold `t` that splits the data into two regions.
   - Predicts the mean of the target values in each region.

3. **Full Tree (Depth ≤ 4)**  
   - Recursively splits the data using the threshold that provides the highest information gain.
   - Stops at a max depth of 4 or when a node has ≤ 1 sample.

4. **Visualization**  
   - Plots the original dataset
   - Overlays predictions from the 1-split decision stump

---

## ▶️ How to Run

1. Install Python 3 (recommended: 3.7 or higher)
2. Install dependencies (if not already installed):

   ```bash
   pip install matplotlib numpy
