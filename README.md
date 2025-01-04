## ML FLow experiements

MLFLOW_TRACKING_URI= \
MLFLOW_TRACKING_USERNAME= \
MLFLOW_TRACKING_PASSWORD= \

import dagshub
dagshub.init(repo_owner='kapilpathak1112', repo_name='mlflow-experiments', mlflow=True)

import mlflow
with mlflow.start_run():
    mlflow.log_param('parameter name', 'value')
    mlflow.log_metric('metric name', 1)
python script.py

