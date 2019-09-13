FROM          docker.elastic.co/elasticsearch/elasticsearch:5.3.0

RUN /usr/share/elasticsearch/bin/elasticsearch-plugin install https://github.com/MLnick/elasticsearch-vector-scoring/releases/download/v5.3.0/elasticsearch-vector-scoring-5.3.0.zip
RUN \
  mv /usr/share/elasticsearch/plugins/x-pack /usr/share/elasticsearch/plugins/.removing-x-pack && \
  mv /usr/share/elasticsearch/plugins/.removing-x-pack /usr/share/elasticsearch/plugins/x-pack && \
  /usr/share/elasticsearch/bin/elasticsearch-plugin remove x-pack
