# mlflow experiments

> Manage MLflow experiments on the tracking server set by `$MLFLOW_TRACKING_URI`.
> See also: `mlflow`, `mlflow runs`.
> More information: <https://mlflow.org/docs/latest/api_reference/cli.html#mlflow-experiments>.

- Create an experiment:

`mlflow experiments create {{[-n|--experiment-name]}} {{experiment_name}}`

- List active experiments:

`mlflow experiments search`

- List all experiments, including deleted ones:

`mlflow experiments search {{[-v|--view]}} all`

- Show details of an experiment by name:

`mlflow experiments get {{[-n|--experiment-name]}} {{experiment_name}}`

- Rename an experiment:

`mlflow experiments rename {{[-x|--experiment-id]}} {{experiment_id}} --new-name {{new_name}}`

- Delete or restore an experiment:

`mlflow experiments {{delete|restore}} {{[-x|--experiment-id]}} {{experiment_id}}`

- Export all runs of an experiment to a CSV file:

`mlflow experiments csv {{[-x|--experiment-id]}} {{experiment_id}} {{[-o|--filename]}} {{path/to/runs.csv}}`
