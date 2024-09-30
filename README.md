# chest-cancer-classification_mlflow_dvc


## Workflows

1. Update config.yaml
2. Update secrets.yaml [Optional] (secret cerdentails or DB details)
3. Update params.yaml (model related params)
4. Update the entity
5. Update the configuration manager in src config
6. Update the components (data prepration, model preparation , model evaluation)
7. Update the pipeline (training and prediction pipeline)
8. Update the main.py (endpoint..to execute pipeline use main.py)
9. Update the dvc.yaml (after implementing the entire peipeline update dvc)


import dagshub
dagshub.init(repo_owner='ashokk.bangaru', repo_name='chest-cancer-classification_mlflow_dvc', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)