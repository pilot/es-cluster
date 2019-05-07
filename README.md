Lazy Ants - elastic search cluster docker configuration
===

You should preinstalled Docker and Docker Compose 

### install

- $> git clone
- $> docker-compose up -d

or run with multiple nodes

- $> docker-compose up -d --scale elasticsearch2=5


### try 

- $> curl -XGET 'http://localhost:9200/lazyants/product/_search' // make a search
- $> curl -XGET 'http://localhost:9200/_cluster/health?pretty=true' // check health status
- $> curl -XGET 'http://localhost:9200/_cat/nodes?v' // node amounts
