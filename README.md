# Apache Airflow Dockerfile

This **Dockerfile** will install [Apache Airflow](https://airflow.incubator.apache.org/) from [PyPi](https://pypi.python.org/pypi) into a container.

### Base Docker Image

* [debian:jessie](https://hub.docker.com/r/library/debian/)


### Installation

1. Install [Docker](https://www.docker.com/).

2. Build the image from Dockerfile: `docker build -t=airflow github.com/ull-isaatc/airflow-docker`

### Usage

    docker run --rm -e LOAD_EX=y -p 8080:8080 airflow webserver

