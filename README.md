# try-airflow
## setup

```shell
$ docker pull apache/airflow:latest
$ docker run -p 8080:8080 -v $(pwd):/opt/airflow/dags -it --rm apache/airflow:latest bash
airflow@0fb2d196762e:~$ airflow initdb
airflow@0fb2d196762e:~$ nohup airflow webserver -p 8080 &
# access to http://localhost:8080
```
