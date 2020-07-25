### Telegraf (Metric) Forwarder

Required environment variables:
  - APP_NAME : Tag of these metrics, used when deployed next to many apps.
  - INFLUX_URL : Full URL with schema and port of your InfluxDB Service "http://influxdb:8086"

```bash
$ docker run -e APP_NAME=my_app -e INFLUX_URL=http://influxdb:8086 -p 8086:8086 telegraf-forwarder:1.0.2
```