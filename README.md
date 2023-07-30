# API-to-Spark-to-HDFS

Purpose
This docker container is meant to be used for learning purpose for programming PySpark. It has the following components.

Hadoop v3.2.1
Spark v2.4.4
Conda 3 with Python v3.7
After running the container, you may visit the following pages.

HDFS
YARN
Spark
Spark History
Jupyter Lab
Airflow
Use docker image

Pull docker image
```
docker pull avnish327030/spark-hadoop-airflow
```
Rename pulled docker image
```
docker image tag  avnish327030/spark-hadoop-airflow spark-hadoop-airflow
```
To run the docker image
window system:

[D:\Project\big_data] is the path and can be replaced based on what you want in below command or you can create this directory and use same command.
```
docker run -it -p 9870:9870 -p 8088:8088 -p 8080:8080 -p 18080:18080 -p 9000:9000 -p 8888:8888 -p 9864:9864 -p 8085:8085 -p 8793:8793 -p 8081:8081 -v D:\project\spark_etl_airflow-main\notebook:/root/ipynb -v D:\project\spark_etl_airflow-main\airflow:/home/airflow -v D:\project\spark_etl_airflow-main\data:/data avnish327030/spark-hadoop-airflow
```
Linux system
```
PROJECT_DIR=$(pwd)
docker run -it 
-p 9870:9870 
-p 8088:8088 
-p 8080:8080 
-p 18080:18080 
-p 9000:9000 
-p 8888:8888 
-p 9864:9864 
-p 8085:8085 
-p 8793:8793 
-p 8081:8081 
-v $PROJECT_DIR/project/notebook:/root/ipynb 
-v $PROJECT_DIR/project/airflow:/home/airflow 
-v $PROJECT_DIR/data:/data 
avnish327030/spark-hadoop-airflow
```

Click on below link to access portal

Name Node

Hadoop Cluster

Spark Master

History Server

Jupyter lab

Hadoop Data Node

Airflow UI

Spark Worker Node
