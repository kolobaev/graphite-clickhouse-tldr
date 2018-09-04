# Quick Start
```sh
git clone https://github.com/vkolobaev/graphite-clickhouse-tldr
cd graphite-clickhouse-tldr
docker-compose up
```
Open http://127.0.0.1:3000/ in browser

### Mapped Ports

Host | Container | Service
---- | --------- | -------------------------------------------------------------------------------------------------------------------
  80 |        80 | carbon-api
3000 |      3000 | grafana
8126 |      8126 | bioyino 
2003 |      2003 | [carbon receiver - plaintext](http://graphite.readthedocs.io/en/latest/feeding-carbon.html#the-plaintext-protocol)
2004 |      2004 | [carbon receiver - pickle](http://graphite.readthedocs.io/en/latest/feeding-carbon.html#the-pickle-protocol)
2006 |      2006 | [carbon receiver - prometheus remote write](https://prometheus.io/docs/prometheus/latest/configuration/configuration/#%3Cremote_write%3E)