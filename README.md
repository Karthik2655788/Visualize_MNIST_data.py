# Visualize_MNIST_data.py

# 🧮 Dimensionality Reduction on Digits Dataset (PCA & t-SNE)

This project demonstrates how to visualize high-dimensional data using **Principal Component Analysis (PCA)** and **t-Distributed Stochastic Neighbor Embedding (t-SNE)** with the `scikit-learn` Digits dataset.

## 📦 Dependencies

Make sure you have the following Python packages installed:

```bash
pip install numpy matplotlib scikit-learn
```

## 📊 Overview

The `load_digits` dataset from `sklearn.datasets` contains 1,797 8×8 images of handwritten digits. Each image is flattened into a 64-dimensional vector.

This project applies:

* **PCA** for linear dimensionality reduction
* **t-SNE** for nonlinear manifold learning

Both techniques reduce the dataset to **2D**, allowing for visualization.

## 🧪 Steps Performed

1. **Load the Dataset**

   * 1797 samples, each of shape (64,)
   * Labels range from 0 to 9 (digits)

2. **PCA Reduction**

   * Reduces data from 64 to 2 dimensions
   * Preserves global linear structure

3. **t-SNE Reduction**

   * Also reduces to 2D
   * Preserves local structure and clusters
   * Parameters: `perplexity=30`, `n_iter=3000`

4. **Visualization**

   * PCA and t-SNE results plotted using `matplotlib`
   * Color-coded by digit labels

## 📷 Sample Output

### PCA Visualization

Displays principal components PC1 vs PC2.

### t-SNE Visualization

Shows better-separated digit clusters by preserving local neighborhoods.

## 🧠 Usage

Run the script:

```bash
python your_script_name.py
```

Replace `your_script_name.py` with the filename.

