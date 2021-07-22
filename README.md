# ELK_SIEM

SIEM is a system that collects information from the private network, analyzes 
and detects malicious behaviors, and shows the records and results to the user 
and manager.

"ELK" is the acronym for three open source projects: Elasticsearch, Logstash, 
and Kibana. Elasticsearch is a search and analytics engine. Logstash is 
a server‑side data processing pipeline that ingests data from multiple sources 
simultaneously, transforms it, and then sends it to a "stash" like 
Elasticsearch. Kibana lets users visualize data with charts and graphs in 
Elasticsearch.

## Pre-requisites

This tools are installed and tested in these following environment:

- Ubuntu OS 20.04
- Docker Container
- ...

## Installation Steps

### Clone Repositories

```shell script
git clone https://github.com/YuxiLing/ELK_SIEM
```

### Run Docker

```shell script
cd <elasticsearch\kibana\logstash>
docker run ...
```

### Check the status
```shell script
docker ps -a
```

### Check the Kibana UI

```
https://localhost:5601
```
## Customizing the Kibana UI for SIEM

### Uploading Kibana Dashboard


### Check the View of the Dashboard