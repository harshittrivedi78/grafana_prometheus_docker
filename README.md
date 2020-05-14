# grafana_prometheus_docker
Docker compose ymls to run grafana and prometheus on your local desktop.

### QuickStart
In prometheus.yml, please update the targets under scrape config. Target should be where your `/metrics` endpoint is exposed. Prometheus will hit this endpoint to scrape the metrics.

To launch the containers
```shell
docker-compose -f monitoring.yml up -d
```
Above command will launch two containers one for prometheus which can be accessed on `http://localhost:9090` and one for grafana which can be reachable on `http://localhost:3030`.
