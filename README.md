# Monitoring Docker-Compose stack

Monitoring software stack for device and http endpoint monitoring with slack alerting.  
Including Grafana, Prometheus, Blackbox, Alertmanager and Prometheus Node Exporter

## Build & Install

```
cp alertmanager/alertmanager.yml.example alertmanager/alertmanager.yml
cp prometheus/prometheus.yml.example prometheus/prometheus.yml
```

You need to supply the slack webhook link in `alertmanager/alertmanager.yml`

```
docker-compose up -d
```

Go to `localhost:3000` in your browser, you can then begin the setup