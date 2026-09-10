https://dagshub.com/SIDHANTBARAPATRE/MLFLOW-AND-DAGSHUB.mlflow

import dagshub
dagshub.init(repo_owner='SIDHANTBARAPATRE', repo_name='MLFLOW-AND-DAGSHUB', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)

