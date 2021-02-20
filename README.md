# Monitoring Docker-Compose stack

[Reference article, credits to M. Franck Bebel](https://medium.com/ouidou/un-monitoring-complet-en-quelques-minutes-avec-prometheus-33e849e6392e)

Monitoring software stack for device and HTTP endpoint monitoring with Slack alerting.

Including Grafana, Prometheus, Blackbox, Alertmanager and Prometheus Node Exporter

## Build & Install

```
cp alertmanager/alertmanager.yml.example alertmanager/alertmanager.yml
cp prometheus/prometheus.yml.example prometheus/prometheus.yml
```

You need to supply the slack webhook link in `alertmanager/alertmanager.yml`

Add HTTP endpoints in the `prometheus/prometheus.yml` file with the same format as the one provided (Prometheus self monitoring) 

```
docker-compose up -d
```

Go to `localhost:3000` in your browser, you can then begin the setup of Grafana