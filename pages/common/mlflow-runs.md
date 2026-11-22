# mlflow runs

> Manage MLflow runs on the tracking server set by `$MLFLOW_TRACKING_URI`.
> See also: `mlflow`, `mlflow experiments`.
> More information: <https://mlflow.org/docs/latest/api_reference/cli.html#mlflow-runs>.

- List the runs of an experiment:

`mlflow runs list --experiment-id {{experiment_id}}`

- List all runs of an experiment, including deleted ones:

`mlflow runs list --experiment-id {{experiment_id}} {{[-v|--view]}} all`

- Print all details of a run as JSON:

`mlflow runs describe --run-id {{run_id}}`

- Create a finished run with a name in an experiment:

`mlflow runs create --experiment-name {{experiment_name}} --run-name {{run_name}}`

- Delete a run:

`mlflow runs delete --run-id {{run_id}}`

- Restore a deleted run:

`mlflow runs restore --run-id {{run_id}}`
