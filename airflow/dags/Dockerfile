# docker build -t image_dbt -f ./airflow/dags/Dockerfile .

FROM ghcr.io/dbt-labs/dbt-postgres:latest

COPY custom_postgres /opt/dbt

COPY .dbt/profiles.yml /root/.dbt/