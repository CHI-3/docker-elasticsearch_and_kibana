## name
docker elasticsearch and kibana

## Overview
sample source for using elasticsearch and kibana on docker

## Versions
- Compose file format 3.7
- elasticsearch 7.7.1
- kibana 7.7.1

## Requirement
- Docker or Docker Toolbox
- curl

## Usage
1. Download and unzip this package and move to the root directory.

2. Start Docker or Docker Toolbox and execute the command below to build the service.
```
docker-compose build --no-cache
```

3. When it's finished, execute the command below to start the containers.
```
docker-compose up -d
```
4. When they started, check that you can connect with them.

#### elasticsearch
execute the command below with your shell.

Docker
```
curl -XGET http://localhost:9200
```
Docker Toolbox
```
curl -XGET http://192.168.99.100:9200
```

#### kibana
execute the command below with your browser.

Docker
```
http://localhost:5601
```
Docker Toolbox
```
http://192.168.99.100:5601
```

5. You can also try sample with data set under "data" directory.

## References
- [Install Elasticsearch with Docker | elastic](https://www.elastic.co/guide/en/elasticsearch/reference/current/docker.html)
- [sugikeitter/elasticsearch-kibana-docker | GitHub](https://github.com/sugikeitter/elasticsearch-kibana-docker)
- [Elasticsearchを日本語で使う設定のまとめ | Qiita](https://qiita.com/shin_hayata/items/41c07923dbf58f13eec4)
