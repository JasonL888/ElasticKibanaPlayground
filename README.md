# ElasticSearch and Kibana "Playground" 

## Overview
"Playground" to try and learn  elasticsearch/kibana on local machine
Using Docker compose to launch official images in separate containers

## Requirements
1. Docker Desktop on Mac

### Launch the containers
```
./startup.sh
```
Internally, this runs the "docker-compose up" in foreground and starts up the containers 

Note: kibana/filebeat have dependencies on elasticsearch so these containers will keep failing/restarting until elasticsearch is fully up - that is expected behavior

### Access Kibana
```
http://localhost:5601
```

### Access Elasticsearch
```
http://localhost:9200
```

### Stop the containers
```
./shutdown.sh
```
