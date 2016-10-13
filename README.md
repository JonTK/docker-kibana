# docker-kibana

This is [Kibana 4.5.4](https://github.com/elastic/kibana) in a minimal 113MB Docker image. Images are tagged by Kibana versions.

[![Docker Repository on Quay.io](https://quay.io/repository/jontk/docker-kibana/status "Docker Repository on Quay.io")](https://quay.io/repository/jontk/docker-kibana)

## Running

```
docker run --name kibana \
           --detach \
           --publish 5601:5601 \
           -e KIBANA_ES_URL=<elasticsearch url> \
           quay.io/jontk/docker-kibana:4.5.4
```

You could set `KIBANA_INDEX` env variable to set an index for Kibana's data.
