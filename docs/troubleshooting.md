# Troubleshooting Runbook

## Cloud Run

Check:

- Service health
- Revision status
- Request errors
- Container logs
- Resource utilization
- Recent deployment changes

## Cloud SQL

Check:

- Instance health
- Connections
- CPU and memory
- Storage
- Database logs
- Recent configuration changes

## Compute Engine

Use Zabbix to review:

- CPU
- Memory
- Disk
- Network
- Availability

## Load Balancer / WAF

Check:

- Backend health
- HTTP/HTTPS status
- Routing configuration
- WAF events
- Certificate status

## Monitoring

Use Grafana for application logs and metrics.

Use Zabbix for VM/infrastructure health.

Check Telegram alert delivery when an alert is triggered.
