FROM conda/miniconda3

RUN mkdir /artifact

RUN pip install mlflow==0.9.0 sqlalchemy psycopg2

CMD ["mlflow", "server", "--backend-store-uri", "postgresql://postgres:example@db/mlflow", "--host", "0.0.0.0", "--default-artifact-root", "/artifact"]