# Healthcare project
# Machine Learning Algorithms in Healthcare
# Table of Contents

- [Project Description](#project-description)
- [Objective](#objective)
- [Methodology](#methodology)
  - [Data Sets](#data-sets)
  - [Tools and Environment](#tools-and-environment)
- [Results](#results)
- [Conclusion](#conclusion)
- [Keywords](#keywords)
#
# Project Description
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




# Projekt Zastosowanie różnych technik uczenia maszynowego do analizy danych medycznych
# Spis Treści

- [Opis Projektu](#opis-projektu)
- [Cel](#cel)
- [Metodologia](#metodologia)
  - [Zbiory Danych](#zbiory-danych)
  - [Narzędzia i Środowisko](#narzędzia-i-środowisko)
- [Wyniki](#wyniki)
- [Wnioski](#wnioski)
- [Słowa Kluczowe](#słowa-kluczowe)
#
# Opis Projektu
Sektor ochrony zdrowia boryka się z wieloma problemami, takimi jak starzenie się społeczeństwa, wypalenie zawodowe i zmęczenie pracowników medycznych, niedobór personelu itp. Algorytmy uczenia maszynowego mogą być cennym narzędziem wspierającym funkcjonowanie tego sektora. Istnieje wiele korzyści wynikających z wykorzystania metod sztucznej inteligencji podczas diagnozy, profilaktyki oraz zarządzania danymi medycznymi pacjentów. Sektor ochrony zdrowia stoi jednak także przed licznymi wyzwaniami i zagrożeniami związanymi z wprowadzeniem narzędzi uczenia maszynowego, ale ich zastosowanie jest konieczne, aby poprawić efektywność pracy oraz zwiększyć poziom bezpieczeństwa pacjentów.

# Cel
Celem tego projektu uczenia maszynowego jest zidentyfikowanie optymalnego algorytmu do klasyfikacji pacjentów na odpowiednie grupy ryzyka dla określonych chorób. Projekt wykorzystuje siedem algorytmów uczenia nadzorowanego (KNN, SVM, random forest, naiwny Bayes, regresja logistyczna i XGBoost) do analizy danych medycznych i identyfikacji kluczowych czynników wpływających na przypisanie do danej grupy ryzyka. Drugim celem analizy było określenie, które cechy są najważniejsze dla konkretnego zbioru danych medycznych. Dodatkowo wykorzystano metody grid search i random search do określenia, który algorytm jest optymalny przy zastosowaniu wielu zbiorów danych i dostosowywaniu hiperparametrów.

# Metodologia
## Zbiory Danych
Zbiory danych obejmują choroby takie jak choroby serca, cukrzyca, choroby wątroby, zakażenie HCV, rak piersi i rak szyjki macicy.

## Narzędzia i Środowisko
Analizę przeprowadzono przy użyciu środowiska Jupyter Notebook i języka programowania Python. W badaniu wykorzystano biblioteki numpy, pandas, sklearn, seaborn i matplotlib. Algorytmy uczenia nadzorowanego to: KNN, SVM, random forest, naiwny Bayes, regresja logistyczna i XGBoost.

# Wyniki
## Wyniki metryki F2 dla algorytmów uczenia nadzorowanego w ocenie wstępnej z użyciem walidacji krzyżowej:

| Zbiór Danych     | KNN  | RF   | CART | NB   | LogR | SVM  | XGB  |
|------------------|------|------|------|------|------|------|------|
| Choroby serca    | 0.67 | 0.83 | 0.76 | 0.81 | 0.82 | 0.84 | 0.86 |
| Cukrzyca         | 0.51 | 0.56 | 0.44 | 0.59 | 0.48 | 0.63 | 0.62 |
| HCV              | 0.76 | 0.79 | 0.63 | 0.63 | 0.65 | 0.70 | 0.91 |
| Choroby wątroby  | 0.78 | 0.86 | 0.85 | 0.48 | 0.88 | 0.85 | 0.80 |
| Rak piersi       | 0.82 | 0.75 | 0.68 | 0.44 | 0.68 | 0.69 | 0.82 |
| Rak szyjki macicy| 0.02 | 0.60 | 0.54 | 0.79 | 0.53 | 0.82 | 0.63 |
| **Średnia**      | 0.59 | 0.7  | 0.65 | 0.62 | 0.67 | 0.76 | 0.77 |

Najlepszy model według oceny wstępnej to XGB (średnia wartość 0.77), następnie SVM (0.76), a na trzecim miejscu RF. Najgorzej wypadł klasyfikator KNN z wynikiem 0.59.

## Wyniki metryki F2 dla algorytmów uczenia nadzorowanego w ostatecznej ocenie na zestawie testowym:

| Zbiór Danych     | KNN  | RF   | CART | NB   | LogR | SVM  | XGB  |
|------------------|------|------|------|------|------|------|------|
| Choroby serca    | 0.84 | 0.83 | 0.89 | 0.82 | 0.83 | 0.84 | 0.82 |
| Cukrzyca         | 0.47 | 0.52 | 0.49 | 0.51 | 0.52 | 0.52 | 0.65 |
| HCV              | 0.81 | 0.93 | 0.91 | 0.71 | 0.79 | 0.80 | 0.89 |
| Choroby wątroby  | 0.74 | 0.74 | 0.49 | 0.41 | 0.62 | 0.52 | 0.92 |
| Rak piersi       | 0.71 | 0.81 | 0.75 | 0.44 | 0.68 | 0.65 | 0.76 |
| Rak szyjki macicy| 0.55 | 0.70 | 0.65 | 0.70 | 0.70 | 0.70 | 0.56 |
| **Średnia**      | 0.69 | 0.76 | 0.70 | 0.60 | 0.69 | 0.67 | 0.77 |

Najlepszy model na podstawie danych testowych to XGB (średnia wartość 0.77), drugi RF (0.76), a trzeci CART (0.70).

## Wyniki AUC dla algorytmów uczenia nadzorowanego w ostatecznej ocenie na zestawie testowym:

| Zbiór Danych     | KNN  | RF   | CART | NB   | LogR | SVM  | XGB  |
|------------------|------|------|------|------|------|------|------|
| Choroby serca    | 0.86 | 0.86 | 0.87 | 0.86 | 0.86 | 0.87 | 0.84 |
| Cukrzyca         | 0.62 | 0.67 | 0.66 | 0.65 | 0.67 | 0.67 | 0.74 |
| HCV              | 0.89 | 0.96 | 0.95 | 0.83 | 0.88 | 0.89 | 0.93 |
| Choroby wątroby  | 0.56 | 0.56 | 0.62 | 0.62 | 0.68 | 0.63 | 0.55 |
| Rak piersi       | 0.76 | 0.70 | 0.66 | 0.69 | 0.62 | 0.72 | 0.70 |
| Rak szyjki macicy| 0.75 | 0.84 | 0.82 | 0.84 | 0.84 | 0.84 | 0.76 |
| **Średnia**      | 0.74 | 0.77 | 0.76 | 0.75 | 0.77 | 0.77 | 0.75 |

Najlepsze wyniki AUC uzyskały modele RF, LogR i SVM (średnia 0.77). 

# Wnioski
W analizie danych medycznych najlepiej sprawdziły się algorytmy zespołowe, takie jak XGBoost, zwłaszcza dla danych niezrównoważonych. Projekt podkreśla znaczenie algorytmów uczenia maszynowego w diagnostyce i leczeniu chorób oraz potrzebę dalszego rozwoju algorytmów sztucznej inteligencji w ochronie zdrowia.

# Słowa Kluczowe:
* uczenie maszynowe, medycyna, ochrona zdrowia, sztuczna inteligencja, KNN, SVM, random forest, naiwny Bayes, regresja logistyczna, XGBoost, RandomSearch, GridSearch.
