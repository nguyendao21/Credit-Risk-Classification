# Credit-Risk-Classification

 Using various techniques to train and evaluate models with imbalanced classes. Using a logistic regression model to compare two versions of the dataset. First, you’ll use the original dataset. Second, you’ll resample the data by using the RandomOverSampler module from the imbalanced-learn library. You will get the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

---

## Technologies

You’ll use [Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/) and the following  **[python version 3.8.5](https://www.python.org/downloads/)** libraries:


* [pandas](https://pandas.pydata.org/docs/)

* [scikit-learn](https://scikit-learn.org/stable/)
    * [scikit metrics](https://scikit-learn.org/stable/modules/model_evaluation.html) 
    *  [imbalanced-learn](https://imbalanced-learn.org/stable/) 
    *  [linear model](https://scikit-learn.org/stable/modules/linear_model.html)

---

## Installation Guide

 ### To check that scikit-learn and hvPlot are installed in your Conda dev environment, complete the following steps:

  ### 1. Activate your Conda dev environment (if it isn’t already) by running the following in your terminal:
```
conda activate dev
```
### 2. When the environment is active, run the following in your terminal to check if the scikit-learn and imbalance-learn libraries are installed on your machine:
```
conda list scikit-learn
conda list imbalanced-learn
```
### If you see scikit-learn and imbalance-learn listed in the terminal, you’re all set!

  ### 1. Install scikit-learn
```
pip install -U scikit-learn
```
### 2. Install imbalance-learn
```
 conda install -c conda-forge imbalanced-learn
```

---



## Usage

To use this application, simply clone the repository and open jupyter lab from git bash by running the following command:

```jupyter lab```

After launching the application, navigate ``credit_risk_resampling`` notebook in the repository. 

Then in your Jupyter notebook, import the required libraries and dependencies.

```
import numpy as np
import pandas as pd
from pathlib import Path
from sklearn.metrics import balanced_accuracy_score
from sklearn.metrics import confusion_matrix
from imblearn.metrics import classification_report_imbalanced
from sklearn.linear_model import LogisticRegression
from imblearn.over_sampling import RandomOverSampler

import warnings
warnings.filterwarnings('ignore')

```




### *Example*

In this application, there are the analysis report using Original Imbalanced Data and Oversample Data

*Classification report for Original Imbalanced Data* 

![original_data](https://user-images.githubusercontent.com/94591580/155906412-e07c26c1-9e56-4931-bc7a-88172a207122.png)


*Classification report for Oversampled Data*

![oversampled_data](https://user-images.githubusercontent.com/94591580/155906438-24429224-6636-446a-894c-901b9cd168f2.png)

---

## Contributors

[Nguyen Dao](https://www.linkedin.com/in/nguyen-dao-a55669215/)

daosynguyen21@gmail.com


---

## License

MIT
