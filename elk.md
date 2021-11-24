# elasticsearch
## [ElasticsearchにCSVファイルの内容をロードする（CSVモジュール ＆ Pandas）](https://kazuhira-r.hatenablog.com/entry/2020/01/01/012853)

## propertyをaggregatableにする
Dev Toolsより以下を実行
```
PUT <index name>/_mapping
{
  "properties": {
    "<property name>": { 
      "type":     "text",
      "fielddata": true
    }
  }
}
```
## dynamic template
https://www.elastic.co/guide/en/elasticsearch/reference/current/dynamic-templates.html

```
PUT index_name/
{
  "mappings": {
    "dynamic_templates": [
      {
        "named_analyzers": {
          "match_mapping_type": "string",
          "match": "text",
          "mapping" : {
           "analyzer" : "kuromoji",
           "fielddata" : true,
           "fields" : {
             "keyword" : {
               "type" : "keyword"
             }
            }
          }
        }
      }
    ]
  }
}
```

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
- [Directly Connecting MySQL DB to Kibana for visualization](https://discuss.elastic.co/t/directly-connecting-mysql-db-to-kibana-for-visualization/239982)
- https://qiita.com/takayuki-miura0203/items/ba9d59a8b267d785d0c6#pipeline

# filebeat
- https://kazuhira-r.hatenablog.com/entry/2019/12/03/001010
- https://www.ossnews.jp/oss_info/Beats/4
- https://dev.classmethod.jp/articles/beats-transform-logstash/

## docker
- https://www.elastic.co/guide/en/beats/filebeat/current/running-on-docker.html
```
docker pull docker.elastic.co/beats/filebeat:7.11.1
```

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTQ1NjgyMTE2NCw4MzM4ODE5NTgsLTM5MD
c5ODE2NywyMTIzMzMyMTIsMzIyMjk2MDAsLTgwMDE0MzA2OCwt
MTU0NDMyNDE1OF19
-->