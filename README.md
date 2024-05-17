# Customer-churn-Classification-using-mlflow

We will classify the customer churn.

* To classify and predict the Customer Churn possibility we are using Random Forest algorithm.
* Create new env
```
conda cretae -n xyz python=3.9 \
pip install -r requirements.txt
```

* Our Architecture would be like

<div align="center">
  <img src="./images/mlflow_mlops_chart.PNG" width="900">
</div>

# Project Structure
bash
```
Copy code
├── data
│   ├── raw
│   ├── processed
├── notebooks
│   ├── data_preprocessing.ipynb
│   ├── model_training.ipynb
│   ├── hyperparameter_tuning.ipynb
│   ├── model_deployment.ipynb
├── scripts
│   ├── preprocess.py
│   ├── train_model.py
│   ├── tune_hyperparameters.py
│   ├── deploy_model.py
├── mlflow
│   ├── mlruns
│   ├── models
├── README.md
└── requirements.txt
```


<br>

## To Do
- [x] Load and preprocess the data
- [x] Model Training
- [x] Hyperparameter tuning with Hyperopt and Mlflow
- [x] Store actifact and metric in Mlflow experimetns
- [x] Evaluate and validate the data
- [x] Deploy model and monitor
- [x] Model Registery from staging to Production

<br>

## Start an MLflow server:
bash
```
mlflow server --backend-store-uri sqlite:///mlflow.db --default-artifact-root ./mlflow/mlruns
```
* Here we started MLflow server and to store data and artifacts we uses sqlite as database



