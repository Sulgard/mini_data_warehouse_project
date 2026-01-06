FROM apache/airflow:2.10.5-python3.12

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

USER root

RUN apt-get update && apt-get install -y build-essential git && apt-get clean

USER airflow

