# CNBC DevOps & GCP Infrastructure

Documentation-only portfolio project describing the CNBC platform infrastructure, environments, deployment architecture, observability, monitoring and alerting.

## Environments

- Production
- Staging
- GCP region: `europe-west3`

## Core GCP Services

- Google Cloud Run
- Cloud SQL for PostgreSQL 17
- Compute Engine
- Cloud Storage
- External Application Load Balancing
- WAF / Cloud Armor
- Grafana
- Zabbix
- Telegram alerting

## Observability

Grafana is used for application and platform logs, metrics and dashboards.

Zabbix is used for VM/infrastructure monitoring such as CPU, memory, disk, network and availability.

Both Grafana and Zabbix are integrated with Telegram for alert notifications.

## Repository Scope

This repository contains architecture and DevOps documentation only. No application source code, credentials, secrets, tokens or production configuration are included.
