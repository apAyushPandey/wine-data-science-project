# Wine Data Science Project

A complete Python-based data science project using the **Wine Recognition Dataset**. The project covers the major stages of a basic data science and machine learning workflow, from data preprocessing and exploratory analysis to feature engineering and model building.

## Project Overview

The Wine Recognition Dataset contains **178 wine samples, 13 numerical chemical features, and 3 wine classes**.

This project is divided into three main stages:

* **Week 1:** Data Acquisition and Pre-processing
* **Week 2:** Exploratory Data Analysis and Visualization
* **Week 3:** Feature Engineering and Model Building

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook / Python

## Week 1 — Data Acquisition and Pre-processing

The first stage focused on acquiring the Wine Recognition Dataset and preparing it for analysis.

Main activities included:

* Dataset acquisition
* Data inspection
* Data cleaning
* Missing-value checking
* Data type checking
* Outlier investigation
* Data normalization and preparation

## Week 2 — Exploratory Data Analysis

The second stage focused on understanding the dataset through statistical analysis and visualization.

Main activities included:

* Summary statistics
* Class distribution analysis
* Feature distributions
* Box plots
* Scatter plots
* Correlation analysis
* Correlation heatmap
* Class-wise comparisons
* Identification of important relationships between features

Important relationships identified included the strong relationship between **total phenols and flavanoids**, as well as useful class-wise differences in alcohol, flavanoids, color intensity, and proline.

## Week 3 — Feature Engineering and Model Building

The third stage extends the EDA findings into machine learning.

### Feature Engineering

Five additional features were created:

1. **Phenolic Ratio**

   * Flavanoids divided by total phenols.

2. **Phenolic Index**

   * Combination of total phenols, flavanoids, and proanthocyanins.

3. **Color-Hue Ratio**

   * Color intensity divided by hue.

4. **Alcohol-Proline Interaction**

   * Interaction between alcohol and proline.

5. **Total Phenol-Flavanoid Interaction**

   * Interaction between total phenols and flavanoids.

These features were created to investigate whether combinations and relationships between chemical measurements could provide useful information for classification.

### Machine Learning Model

**Logistic Regression** was selected as the baseline classification algorithm.

The workflow includes:

* Train-test splitting
* Feature scaling using `StandardScaler`
* Logistic Regression training
* Prediction on test data
* Model evaluation
* 5-fold cross-validation

### Evaluation Metrics

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix
* 5-fold Cross-Validation

The feature-engineering experiment demonstrated that adding features does not automatically improve model performance. This provides a useful practical lesson about evaluating engineered features objectively.

## Project Structure

```text
wine-data-science-project/
│
├── Week 1/
│   └── Data Acquisition and Pre-processing
│
├── Week 2/
│   └── Exploratory Data Analysis and Visualization
│
├── Week 3/
│   ├── Week_3_Feature_Engineering_and_Model_Building_Wine.docx
│   ├── week3_model.py
│   └── outputs/
│       ├── accuracy_comparison.png
│       ├── confusion_matrix.png
│       └── feature_count.png
│
└── README.md
```

## Results

The Week 3 experiment compared a baseline Logistic Regression model with a model containing engineered features.

The evaluation showed that the original features already provided strong predictive information. Feature engineering was useful for testing additional representations of the data, but the engineered features did not produce a significant improvement over the baseline model.

## Future Improvements

Future work can include:

* Decision Tree classification
* Random Forest classification
* Support Vector Machine
* K-Nearest Neighbors
* Hyperparameter tuning
* Feature selection
* Principal Component Analysis (PCA)
* Cross-validation comparison
* More advanced feature engineering

## Conclusion

This project demonstrates a complete beginner-friendly data science workflow using the Wine Recognition Dataset. It progresses from data acquisition and preprocessing to exploratory analysis, feature engineering, machine learning, and model evaluation.

The project also demonstrates that machine learning improvements should be supported by measurable results rather than assumptions.

## References

* Scikit-learn documentation
* UCI Machine Learning Repository
* Pandas documentation
* NumPy documentation
* Matplotlib documentation
