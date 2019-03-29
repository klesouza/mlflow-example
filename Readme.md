- Creates a MLFlow Tracking serving server using a PostgresSQL as store
- Runs a model and report to the server

### TODO
- Initialize database (create `mlflow` if not exists)
- Model container has to wait the tracking server to be ready
- Improve `model` not to reacreate the `conda` envrionment every run (perhaps change to `docker_env` version)