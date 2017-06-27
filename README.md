# Apache Airflow Dockerfile

This **Dockerfile** will install [Apache Airflow](https://airflow.incubator.apache.org/) from [PyPi](https://pypi.python.org/pypi) into a container.

### Base Docker Image

* [debian:jessie](https://hub.docker.com/r/library/debian/)


### Installation

1. Install [Docker](https://www.docker.com/).

2. Download [PostgresSQL container](https://hub.docker.com/_/postgres/) from public [Docker Hub Registry](https://registry.hub.docker.com/): `docker pull postgres`

3. Build the image from Dockerfile: `docker build -t=airflow github.com/ull-isaatc/airflow-docker`

### Usage

    # docker run --name some-postgres -e POSTGRES_USER=airflow -e POSTGRES_PASSWORD=airflow -e POSTGRES_DB=airflow -d postgres
    # docker run --name some-airflow  -e LOAD_EX=y -p 8080:8080 airflow webserver

