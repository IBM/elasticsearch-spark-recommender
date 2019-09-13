#### 2.0 Start Elasticsearch with docker
If you familier with docker you can use the [elasticsearch docker image](https://www.elastic.co/guide/en/elasticsearch/reference/current/docker.html) with installed elasticsearch-vector-scoring plugin.
Just go to docker/elasticsearch/ directory where you can find the ```Dockerfile``` and build the image with
```docker build -t es-with-vector-scoring .``` command. 
Check that the image is successfully built:
```
$ docker build -t es-with-vector-scoring .
  Sending build context to Docker daemon   5.12kB
  Step 1/3 : FROM          docker.elastic.co/elasticsearch/elasticsearch:5.3.0
  ...
  Successfully built 53ee57082cb8
  Successfully tagged es-with-vector-scoring:latest
```


If builds ended you can start the image with ```docker run -p 9200:9200 -p 9300:9300 es-with-vector-scoring``` command. 
Check that the `elasticsearch-vector-scoring-plugin` is successfully loaded and elasticsearch is started:

```
$ docker run -p 9200:9200 -p 9300:9300 es-with-vector-scoring
  [2018-05-09T18:58:24,901][INFO ][o.e.n.Node               ] [] initializing ...
 ...
  [2018-05-09T18:58:29,089][INFO ][o.e.p.PluginsService     ] [Zs-WKd8] loaded plugin [elasticsearch-vector-scoring]
 ...
  [2018-05-09T18:58:36,108][INFO ][o.e.n.Node               ] [Zs-WKd8] started
 ...
```

Now that you've got Elasticsearch up and running, you can go back to step 2.2.
