
# [ElasticsearchにCSVファイルの内容をロードする（CSVモジュール ＆ Pandas）](https://kazuhira-r.hatenablog.com/entry/2020/01/01/012853)

# docker-compose
docker-compose.yaml 
```yaml
version: '2'

services:
  elasticsearch:
    image: docker.elastic.co/elasticsearch/elasticsearch-oss:7.2.0
    volumes:
      - elasticsearch-data:/usr/share/elasticsearch/data
    ports:
      - 9200:9200
    expose:
      - 9300
    environment:
      - discovery.type=single-node
      - "ES_JAVA_OPTS=-Xms2048m -Xmx2048m"
  kibana:
    image: docker.elastic.co/kibana/kibana-oss:7.2.0
    ports:
      - 5601:5601

volumes:
  elasticsearch-data:
    driver: local
```

# [Kibana×ElasticSearchをConoHa(512MB)で動かす](https://country-dev.hatenablog.com/entry/2017/09/25/000759)

# can directly connect mysql
[Directly Connecting MySQL DB to Kibana for visualization](https://discuss.elastic.co/t/directly-connecting-mysql-db-to-kibana-for-visualization/239982)

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE0MjUyNjQxMTBdfQ==
-->