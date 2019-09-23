# behavior_modelling_workshop
Comparison of various Classification models for mode choice
This repository contains the code used in Mode choice prediction using Traditional and Machine Learning methods.

### Requirements

* Python == 3.6.7
* Tensorflow == 1.14.0
* Keras == 2.2.4
* Scipy == 1.2.1
* Statsmodels == 0.9.0
* Sci-kit learn == 0.21.1

### Dataset #1

Person Trip (PT) data `PT_NEW_without_unknowns.zip` for city of Yokohama is used. After data cleaning and removal of entries with empty values,
the dataset consists of `1443009` entries. The complete dataset is divided into 2 parts as `Train` and `Test` set in the ratio `85:15`.


### Dataset #2

Person Probe (PP) data `PP_Data_Clean_English_new.csv` for city of Yokohama is also used in the study. After data cleaning, the dataset consists of `1522` entries.
Further, the dataset is divided into 2 parts as `Train` and `Test` set in the ratio `70:30`.

### Prediction models

* Multinomial Logit (MNL) is utilised from statsmodel library.
* Random Forests (RF) from Sci-kit learn.
* Extreme Gradient Boosting (XGB) from xgboost.
* Artificial Neural Networks (ANN) from Keras.

### Tips to reiterate the Notebook

* Extract PT-data csv file from `PT_NEW_without_unknowns.zip`.
* All the four models tested for each of the datasets and are given as single notebook.
- `PT_data_analysis-overall.ipynb` corresponds to PT data analysis.
- `PP_data_analysis-overall.ipynb` corresponds to PP data analysis.

### Notes

* `Train` and `Test` data used in each model is same, therefore the metrics obtained from such models can be compared with each other.
* `MNL` model is used in this exercise only to predict the mode choice behavior in this stuy and not to study interaction between predictor variables.
