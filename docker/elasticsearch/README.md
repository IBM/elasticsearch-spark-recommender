#### 2.0 Start Elasticsearch with docker
If you familier with docker you can use the elasticsearch docker image with installed elasticsearch-vector-scoring plugin.
Just build the image with 
```docker build es-with-vector-scoring```
and start the image with ```docker run -p 9200:9200 -p 9300:9300 elasticsearch-vector-scoring```
