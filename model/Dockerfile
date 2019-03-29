FROM conda/miniconda3

RUN apt update && apt install -y git-all
RUN pip install mlflow==0.9.0 && mkdir /model
WORKDIR /model
COPY . /model

CMD ["mlflow", "run", "."]