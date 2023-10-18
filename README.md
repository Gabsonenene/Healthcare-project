# Healthcare project
# Project Description: Machine Learning Algorithms in Healthcare

The health care sector is facing numerous problems, such as an aging population, burnout and fatigue of medical workers, staff shortages, etc. Machine learning algorithms can be a valuable tool supporting the functioning of this sector. There are numerous benefits resulting from the use of artificial intelligence methods during diagnosis, prevention and management of patients' medical data. The healthcare sector faces numerous challenges and threats resulting from the introduction of machine learning tools, but these tools are necessary to improve work efficiency and increase the level of patient safety.

# Objective
This machine learning project aims to identify the optimal algorithm for classifying patients into appropriate risk groups for specific diseases. The project leverages seven supervised learning algorithms (KNN, SVM, random forest, naïve Bayes, logistic regression, and XGBoost) to analyze medical data and identify key factors influencing the inclusion in a given risk group. A second goal of the analysis was to determine which features are most important for a specific medical dataset. In addition, grid search and random search methods were used to determine which algorithm is optimal when using multiple datasets and adjusting hyperparameters.

# Methodology
## Data Sets
The datasets include diseases such as heart disease, diabetes, liver disease, HCV infection, breast cancer and cervical cancer.

## Tools and Environment
This analysis was carried out using a Jupyter Notebook and Python programming language. In this study, numpy, pandas, sklearn, seaborn, and matplotlib libraries were used. Supervised learning algorithms: KNN, SVM, random forest, naïve Bayes, logistic regression, and XGBoost.

# Results
## F2 metric scores for supervised learning algorithms in preliminary evaluation using cross-validation:

| Dataset         | KNN  | RF   | CART | NB   | LogR | SVM  | XGB  |
|-----------------|------|------|------|------|------|------|------|
| Heart disease   | 0.67 | 0.83 | 0.76 | 0.81 | 0.82 | 0.84 | 0.86 |
| Diabetest       | 0.51 | 0.56 | 0.44 | 0.59 | 0.48 | 0.63 | 0.62 |
| HCV             | 0.76 | 0.79 | 0.63 | 0.63 | 0.65 | 0.70 | 0.91 |
| Liver disease   | 0.78 | 0.86 | 0.85 | 0.48 | 0.88 | 0.85 | 0.80 |
| Breast cancer   | 0.82 | 0.75 | 0.68 | 0.44 | 0.68 | 0.69 | 0.82 |
| Cervical cancer | 0.02 | 0.60 | 0.54 | 0.79 | 0.53 | 0.82 | 0.63 |
| **Mean**        | 0.59 | 0.7  | 0.65 | 0.62 | 0.67 | 0.76 | 0.77 |

According to a preliminary assessment of classification quality, the best model was XGB with an average value of 0.77, followed by SVM with an average value of 0.76, and in third place was RF. The worst performer was the KNN classifier with an average value of 0.59.

## Results of F2 metrics for supervised learning algorithms for the final evaluation based on the test set:

| Dataset         | KNN  | RF   | CART | NB   | LogR | SVM  | XGB  |
|-----------------|------|------|------|------|------|------|------|
| Heart disease   | 0.84 | 0.83 | 0.89 | 0.82 | 0.83 | 0.84 | 0.82 |
| Diabetest       | 0.47 | 0.52 | 0.49 | 0.51 | 0.52 | 0.52 | 0.65 |
| HCV             | 0.81 | 0.93 | 0.91 | 0.71 | 0.79 | 0.80 | 0.89 |
| Liver disease   | 0.74 | 0.74 | 0.49 | 0.41 | 0.62 | 0.52 | 0.92 |
| Breast cancer   | 0.71 | 0.81 | 0.75 | 0.44 | 0.68 | 0.65 | 0.76 |
| Cervical cancer | 0.55 | 0.70 | 0.65 | 0.70 | 0.70 | 0.70 | 0.56 |
| **Mean**        | 0.69 | 0.76 | 0.70 | 0.60 | 0.69 | 0.67 | 0.77 |

Based on the results obtained for the classification for the test data, the best model was XGB with a mean value of 0.77, followed by RF (0.76) in second place, and in third place was CART (0.70).

## AUC results for supervised learning algorithms for final evaluation based on the test set:

| Dataset          | KNN   | RF    | CART  | NB    | LogR  | SVM   | XGB   |
|------------------|-------|-------|-------|-------|-------|-------|-------|
| Heart disease    | 0.86  | 0.86  | 0.87  | 0.86  | 0.86  | 0.87  | 0.84  |
| Diabetest        | 0.62  | 0.67  | 0.66  | 0.65  | 0.67  | 0.67  | 0.74  |
| HCV              | 0.89  | 0.96  | 0.95  | 0.83  | 0.88  | 0.89  | 0.93  |
| Liver disease    | 0.56  | 0.56  | 0.62  | 0.62  | 0.68  | 0.63  | 0.55  |
| Breast cancer    | 0.76  | 0.70  | 0.66  | 0.69  | 0.62  | 0.72  | 0.70  |
| Cervical cancer  | 0.75  | 0.84  | 0.82  | 0.84  | 0.84  | 0.84  | 0.76  |
| **Mean**         | 0.74  | 0.77  | 0.76  | 0.75  | 0.77  | 0.77  | 0.75  |

Based on the ROC curve, the best results were obtained by the models: RF, LogR, and SVM (mean 0.77), followed by CART (0.76). In third place were XGB and NB models (0.75), and the lowest average AUC value was obtained by the KNN model.

In the final analysis, the best results were obtained for the XGBoost, RF, and CART models for the F2 metric. In the case of imbalanced data, the CART model performed best.

# Conclusion
For medical data analysis, ensemble learning algorithms such as XGBoost have been shown to perform best, especially for imbalanced data.
This project highlights the importance of machine learning algorithms in the diagnosis and treatment of diseases and emphasizes the need for further development of artificial intelligence algorithms in health care.

# Keywords: 
* machine learning, medicine, healthcare, artificial intelligence, KNN, SVM, random forest, naïve Bayes, logistic regression, XGBoost, RandomSearch, GridSearch.