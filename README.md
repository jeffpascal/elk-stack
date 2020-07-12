# elk-stack
 elastic search/ kibana/ logstash trying


## Resource srping with elk

https://dzone.com/articles/sprinkle-some-elk-on-your-spring-boot-logs

## Docker setup

1. Elastic search

- Pulling the image

- Obtaining Elasticsearch for Docker is as simple as issuing a docker pull command against the Elastic Docker registry.

```docker pull docker.elastic.co/elasticsearch/elasticsearch:7.8.0```

- Alternatively, you can download other Docker images that contain only features available under the Apache 2.0 license. To download the images, go to www.docker.elastic.co.

### Starting a single node cluster with Dockeredit

To start a single-node Elasticsearch cluster for development or testing, specify [single-node](https://www.elastic.co/guide/en/elasticsearch/reference/current/bootstrap-checks.html#single-node-discovery) discovery to bypass the [bootstrap checks:](https://www.elastic.co/guide/en/elasticsearch/reference/current/bootstrap-checks.html)

```docker run -p 9200:9200 -p 9300:9300 -e "discovery.type=single-node" docker.elastic.co/elasticsearch/elasticsearch:7.8.0```

### Starting a multi-node server 

- https://www.elastic.co/guide/en/elasticsearch/reference/current/docker.html


