Consul Based Discovery Plugin for Elasticsearch
======================================

Uses [Consul](https://consul.io) API for Elasticsearch discovery


## Configuration

```
discovery:
  type: consul
  consul:
    service-names: ["CONSUL_SERVICE_NAME1", "CONSUL_SERVICE_NAME2"]
    tag:  OPTIONAL_TAG_TO_FILTER_NODES
    api-host: OPTIONAL_CONSUL_HTTP_API_HOSTNAME_DEFAULT_IS_LOCALHOST
    api-port:  OPTIONAL_CONSUL_HTTP_API_PORT_FOR_CONSUL_DEFAULT_IS_8500

```


This plugin is based on https://github.com/grantr/elasticsearch-srv-discovery and
modified to be based on consul API calls instead of DNS records.
