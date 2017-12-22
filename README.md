## Description
  test project for kibana.  

## Usage
  clone this project.  
```bash
$ git clone this_project_url
$ cd /path/to/this-project
$ docker-compose up
```

  ready sample json data.  
  and then pour it into elasticsearch.  
```bash
$ docker cp sample.json kibanasample_elasticsearch_1:/usr/share/elasticsearch
$ docker exec -it kibanasample_elasticsearch_1 bash
$ curl -s -XPOST localhost:9200/_bulk --data-binary sample.json
```
