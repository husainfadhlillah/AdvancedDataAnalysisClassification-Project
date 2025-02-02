# 🎯 Statistical Inference Project - Advanced Data Analysis and Classification

## 📊 Project Overview
This project demonstrates a comprehensive statistical analysis and machine learning classification approach on a dataset, focusing on proper data sampling, distribution analysis, normality testing, and parameter tuning.

## 🔍 Key Features
- Data sampling and distribution analysis
- Normality testing using Kolmogorov-Smirnov method
- Data transformation techniques
- Machine learning classification with parameter tuning
- Hypothesis testing for model evaluation

## 🛠️ Technologies Used
- Python 3.x
- Libraries:
  - 📈 pandas & numpy for data manipulation
  - 📊 matplotlib & seaborn for visualization
  - 🧪 scipy for statistical tests
  - 🤖 scikit-learn for machine learning
  - 🔄 TPOT for automated machine learning

## 📝 Project Structure
1. **Data Preparation & Analysis**
   - 80:20 train-test split
   - Distribution analysis between training and overall data
   - Visualization using histograms and KDE plots

2. **Normality Testing**
   - Kolmogorov-Smirnov test implementation
   - Multiple transformation methods tested:
     - Box-Cox transformation
     - Log transformation
     - Square Root transformation
     - Arc Sin transformation
     - Yeo-Johnson transformation

3. **Classification Model**
   - Random Forest Classifier implementation
   - Feature scaling using StandardScaler
   - Dimensionality reduction using FastICA

4. **Parameter Tuning**
   - Parameters tested:
     - n_estimators: [50, 100, 150, 200]
     - min_samples_leaf: [1, 2, 4, 6]
   - 5 iterations per parameter combination
   - Results tabulation and analysis

5. **Hypothesis Testing**
   - One-way ANOVA for parameter significance
   - 95% confidence level testing
   - Analysis of parameter impact on model accuracy

## 📈 Results
- Comprehensive normality analysis across different transformation methods
- Detailed parameter tuning results with accuracy metrics
- Statistical significance testing of parameter effects
- ANOVA results for model parameter evaluation

## 🎓 Key Findings
- Yeo-Johnson transformation showed optimal results for data normalization
- No significant difference found in model performance across different parameter values (95% confidence level)
- Random Forest classifier demonstrated stable performance across multiple iterations

## 📚 How to Use
1. Install required dependencies:
```python
pip install pandas numpy scipy sklearn matplotlib seaborn tpot
```

2. Load and prepare your dataset:
```python
data = pd.read_excel('your_dataset.xlsx')
```

3. Run the analysis pipeline:
```python
# Data splitting
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

# Apply transformations and run classification
# (See detailed code in notebook)
```

## ✨ Conclusion
This project demonstrates a robust approach to statistical analysis and machine learning classification, with careful attention to data distribution, transformation, and parameter optimization. The results provide insights into the effectiveness of different transformation methods and the impact of model parameters on classification performance.
