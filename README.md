# DNA Binding Sites Prediction
Second Project of the Machine Learning course in collaboration with the EPFL Laboratory for Computation and Visualization in Mathematics and Mechanics.

# File Structure
* `code` - Folder containing training utilities
  * `metrics_helper.py` - Utilities for performance measures.
  * `preprocessing_helper.py` - Helper for preprocessing the data.
  * `sampling_helper.py` - Implementation of the undersampling and oversampling experimented strategies.
  * `Best Run Regression.ipynb` - Notebook for reproducibility of regression results.
  * `Best_Run_classification.ipynb` - Notebook for reproducibility of classification results.
* `data` - Link to the original dataset
* `report.pdf` - Report pdf file
* `requirements.txt` - Requirements text file

## Reproducibility
### Optimal Parameters (Regression)
To reproduce the results we obtained for the regression task, please use a **XGBoost Regressor** model with the following hyperparameters:
```python
parameters = {'subsample' : 0.8999999999999999,
              'n_estimators' : 500,
              'max_depth' : 20,
              'learning_rate' : 0.01,
              'colsample_bytree' : 0.7999999999999999,
              'colsample_bylevel' : 0.6}
```

### Optimal Parameters(Classification)
To reproduce the results we obtained for the classification task, please use a **Random Forest Classifier** with the following hyperparameters:
```python
parameters = {'n_estimators':400,
              'min_samples_split':5,
              'min_samples_leaf':1,
              'max_features':'auto',
              'max_depth':20,
              'bootstrap':False}
```

## Report
The report can be found in pdf format in the `report` folder.

## Authors
- Federico Betti
- Ioannis Mavrothalassitis
- Luca Rossi
