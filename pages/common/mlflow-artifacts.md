# mlflow artifacts

> Upload, list, and download artifacts of MLflow runs.
> See also: `mlflow`, `mlflow runs`.
> More information: <https://mlflow.org/docs/latest/api_reference/cli.html#mlflow-artifacts>.

- List the artifacts at the root of a run:

`mlflow artifacts list {{[-r|--run-id]}} {{run_id}}`

- List the artifacts in a directory of a run:

`mlflow artifacts list {{[-r|--run-id]}} {{run_id}} {{[-a|--artifact-path]}} {{path/to/directory}}`

- Upload a local file as an artifact of a run:

`mlflow artifacts log-artifact {{[-l|--local-file]}} {{path/to/file}} {{[-r|--run-id]}} {{run_id}}`

- Upload all files in a local directory into a directory of a run:

`mlflow artifacts log-artifacts {{[-l|--local-dir]}} {{path/to/directory}} {{[-r|--run-id]}} {{run_id}} {{[-a|--artifact-path]}} {{path/to/artifact_directory}}`

- Download all artifacts of a run to a local directory:

`mlflow artifacts download {{[-r|--run-id]}} {{run_id}} {{[-d|--dst-path]}} {{path/to/directory}}`

- Download an artifact by its URI to a temporary directory and print its local path:

`mlflow artifacts download {{[-u|--artifact-uri]}} runs:/{{run_id}}/{{path/to/artifact}}`
