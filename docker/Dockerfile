FROM apache/airflow:2.3.4
USER root
RUN apt-get update \
    && apt-get install -y --no-install-recommends \
    vim \
    && apt-get autoremove -yqq --purge \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
USER airflow

FROM apache/airflow:2.3.4
RUN pip install --no-cache-dir scikit-learn
