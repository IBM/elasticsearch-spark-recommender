# Building a Recommender with Apache Spark & Elasticsearch

This repo contains demo Jupyter notebooks illustrating the basics of how to use Apache Spark for generating ALS models from ratings data stored in Elasticsearch, saving the model factors to ES, and then using ES to serve real-time recommendations using the user and item factors.

### Requirements

* `elasticsearch-spark` JAR (version `5.3.0`) on the classpath ([download](https://www.elastic.co/downloads/past-releases/elasticsearch-apache-hadoop-5-3-0)).
* Spark 2.1.x ([download](http://spark.apache.org/downloads.html)).
* Running instance of Elasticsearch 5.3.0 ([download](https://www.elastic.co/downloads/past-releases/elasticsearch-5-3-0)).
* Elasticsearch vector scoring plugin installed (https://github.com/MLnick/elasticsearch-vector-scoring).
* Jupyter (`pip install jupyter`).

To run: 

```
PYSPARK_DRIVER_PYTHON=ipython PYSPARK_DRIVER_PYTHON_OPTS="notebook" PATH_TO_SPARK_2.1/bin/pyspark --driver-memory 2g --jars PATH_TO_ES_HADOOP/dist/elasticsearch-spark_2.11-5.3.0.jar
```
