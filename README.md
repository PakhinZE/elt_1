Tool
	- PostgreSQL
	- Docker
	- dbt
	- Airflow

move .dbt folder to home directory\
when change elt_dag.py need to rebuild elt-custom_dbt\
AIRFLOW__WWW_USER_USERNAME: airflow\
AIRFLOW__WWW_USER_PASSWORD: password

docker compose up init-airflow -d\
docker compose up

docker compose down -v

# check correctness
docker exec -it elt-destination_postgres-1 psql -U postgres\
\c destination_db\
\dt\
SELECT * FROM specific_movie;
