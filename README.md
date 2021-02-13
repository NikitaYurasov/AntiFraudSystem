# AntiFraudSystem

This project was made for development the AI antifraud system using ML.

For mostly all antifraud systems it is more important not to block legitimate transaction, but to verify as much as possible fraud transactions.

```
Training dataset was not uploaded into this repository because of security considerations and big volume.
All personal data, that is used in the project, was hashed before any calculations and uploading.
If you want to prove or contribute my work, please contact me for getting data.
```

## Primary task was:
### Main steps of the project
1. Collect data, aggregate and transfer into that form, that would be useful and complete for further exploration.
2. Feature engineering: try to understand the underlying data; find out new feautures from input datasets; extimate contribution to predict target variable
3. Find the best model, that can predict most correctly fraud transactions.

The following restrictions apply to the model:
- perfect model is based on the tree algorithms (RandomForest was taken as the base model)
- all metrics should be calculated according to the fraud transactions (there is obvious and logic classes imbalance)

## Metrics

Selected task is binary classification, where target variable can be 0 (not fraud) or 1 (fraud). 

As final metric, **recall** was taken and there is information about previous model: 0.1 - precision and 0.3 - recall according to the positive class.

Main goal was to increase recall metric.

```
Metric for simulation and tuning hyperparameters was taken **F1 Score**, 
due to the fact that it's the best way of estimation precision and recall at the same time&
```

## TODO
1. Use HYPERopt & Ray Tune for parameters tuning and decline the RandomGridSearch
2. Try Boosting algorithms (further exploration with big amount of data)
