# Perceptron with Feature Engineering and Convergence Analysis

## Project-Based Learning (PBL) – Pattern Matching

### 1. Project Overview

This project focuses on developing a Perceptron Classifier with Feature Engineering and analyzing its learning behavior using the Iris dataset.

The primary objective is to understand how feature engineering influences classification performance, learning convergence, misclassification rate, and decision boundaries.

A Perceptron model is implemented from scratch using Python and NumPy. Original features are compared with polynomial features to study their impact on the model's learning process and classification performance.

### 2. Project Aim

To develop a perceptron classifier with engineered features and analyze learning convergence, misclassification, and decision boundaries.

### 3. Objectives

- Implement a Perceptron classifier from scratch.
- Understand weights, bias, activation functions, and the learning rate.
- Perform feature engineering using polynomial features.
- Analyze model convergence across multiple training epochs.
- Calculate classification accuracy and misclassification rates.
- Visualize decision boundaries for original and engineered features.
- Evaluate model performance using a confusion matrix.
- Study the effect of different learning rates on convergence.

### 4. Dataset Description

**Dataset:** Iris Dataset

The Iris dataset is a popular machine learning dataset containing 150 flower samples belonging to three species.

| Feature | Description |
|---|---|
| Sepal Length | Length of the sepal in cm |
| Sepal Width | Width of the sepal in cm |
| Petal Length | Length of the petal in cm |
| Petal Width | Width of the petal in cm |
| Target | Iris flower species |

**Classification Approach:**

The main experiment uses binary classification:

- Setosa: Class -1
- Versicolor: Class +1

The Versicolor and Virginica species are also used in a separate experiment to investigate classification difficulty and convergence.

### 5. Technologies Used

- Python
- Google Colab
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

### 6. Methodology

The project follows these steps:

1. **Dataset Loading:** Load and explore the Iris dataset.
2. **Data Preprocessing:** Select the required species and numerical features.
3. **Train-Test Splitting:** Divide the dataset into training and testing sets.
4. **Feature Scaling:** Apply StandardScaler to normalize the input features.
5. **Perceptron Implementation:** Implement the learning algorithm using NumPy.
6. **Feature Engineering:** Generate polynomial features of degree two.
7. **Model Training:** Train perceptron models using original and engineered features.
8. **Convergence Analysis:** Track training misclassifications across epochs.
9. **Performance Evaluation:** Calculate accuracy and generate a confusion matrix.
10. **Visualization:** Plot convergence curves and decision boundaries.

### 7. Perceptron Learning Algorithm

The perceptron calculates the weighted sum of input features:

z = w1x1 + w2x2 + b

The prediction is determined by:

- If z >= 0, predict class +1.
- If z < 0, predict class -1.

**Weight Update Rule:**

w = w + learning_rate * y * x

b = b + learning_rate * y

The weights and bias are updated whenever a sample is misclassified or lies on the decision boundary.

### 8. Feature Engineering

Polynomial feature engineering is applied to the original input features.

For two input features x1 and x2, the generated features include:

- x1
- x2
- x1²
- x1 * x2
- x2²

These additional features enable the perceptron to learn more complex decision boundaries in the original feature space.

### 9. Experiments Performed

| Experiment | Description |
|---|---|
| Experiment 1 | Train perceptron using original features |
| Experiment 2 | Apply polynomial feature engineering |
| Experiment 3 | Compare original and engineered features |
| Experiment 4 | Analyze convergence across epochs |
| Experiment 5 | Study different learning rates |
| Experiment 6 | Investigate a more challenging Iris classification problem |

### 10. Performance Evaluation

The following evaluation methods are used:

- **Accuracy:** Percentage of correctly classified samples.
- **Misclassification Rate:** Percentage of incorrectly classified samples.
- **Convergence Analysis:** Number of epochs required to reach zero training errors.
- **Confusion Matrix:** Comparison between actual and predicted class labels.
- **Decision Boundary:** Visualization of the classification regions.

### 11. Visualizations

The project generates the following graphs:

1. Iris dataset distribution.
2. Perceptron convergence curve.
3. Original-feature decision boundary.
4. Polynomial-feature decision boundary.
5. Confusion matrix.
6. Learning-rate comparison graph.
7. Convergence analysis for Versicolor and Virginica.

### 12. Project Results

The project evaluates the effect of feature engineering on perceptron learning.

The results are analyzed by comparing:

- Original features versus polynomial features.
- Training convergence and misclassification.
- Test classification accuracy.
- Decision boundary behavior.
- Learning-rate impact.

**Note:** Actual accuracy, convergence epochs, and misclassification values should be added after executing the Google Colab notebook.

### 13. How to Run the Project

**Step 1:** Clone the repository.

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

**Step 2:** Open Google Colab.

https://colab.research.google.com/

**Step 3:** Upload the project notebook:

`Perceptron_Feature_Engineering_PBL.ipynb`

**Step 4:** Run all cells sequentially.

**Step 5:** Observe the generated graphs, evaluation metrics, and experimental results.

### 14. Project Structure

```text
Perceptron-Feature-Engineering/
│
├── Perceptron_Feature_Engineering_PBL.ipynb
│
├── outputs/
│   ├── convergence_analysis.png
│   ├── confusion_matrix.png
│   ├── challenging_convergence.png
│   └── learning_rate_comparison.png
│
├── perceptron_experiment_results.csv
├── perceptron_convergence_history.csv
│
└── README.md
```

### 15. Conclusion

This project demonstrates the implementation of a Perceptron Classifier and the importance of feature engineering in pattern classification.

By comparing original features with polynomial features, the project investigates changes in classification performance and decision boundaries.

The convergence analysis provides insights into how a perceptron learns from training data and demonstrates the relationship between linear separability and convergence.

Overall, the project provides practical understanding of perceptron learning, feature transformation, classification, and pattern recognition.

### 16. Future Enhancements

- Extend binary classification to multiclass classification.
- Experiment with additional feature transformations.
- Compare perceptron performance with logistic regression and other classifiers.
- Develop an interactive dashboard for visualizing decision boundaries.
- Investigate the impact of noise and different dataset sizes.

---

**Project Domain:** Machine Learning / Pattern Recognition

**Subject:** Pattern Matching

**Project Type:** Project-Based Learning (PBL)

**Dataset:** Iris Dataset

**Development Platform:** Google Colab
