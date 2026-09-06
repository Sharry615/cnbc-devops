# CNBC Architecture

## High-Level Architecture

```text
                         INTERNET
                             |
                             v
                  External HTTPS Load Balancer
                             |
                             v
                       WAF / Cloud Armor
                             |
          +------------------+------------------+
          |                  |                  |
          v                  v                  v
     Cloud Run           Cloud Run         Cloud Storage
     Frontends           Backends          / Assets
          |                  |
          +---------+--------+
                    |
                    v
              Cloud SQL PostgreSQL
                    |
                    |
              Compute Engine
             cnbc-analytics


              OBSERVABILITY
                    |
        +-----------+-----------+
        |                       |
        v                       v
     Grafana                  Zabbix
 Logs + Metrics          VM / Infrastructure
 Dashboards              CPU / Memory / Disk
        |                       |
        +-----------+-----------+
                    |
                    v
                 Telegram
                  Alerts
```

## Production

Production contains separate Cloud Run services for admin, client frontend, news and ZagTrader workloads.

## Staging

Staging contains separate Cloud Run services for admin frontend/backend, client frontend and news.

## Load Balancing

The supplied console screenshots show multiple external Application Load Balancers using HTTPS/HTTP and routing to Cloud Run backend services and backend buckets.

## Database

Production and staging use separate Cloud SQL PostgreSQL 17 instances.

## VM

`cnbc-analytics` is deployed on Compute Engine in `europe-west3-a`.

## Public Portfolio Safety

Public documentation must not include:

- Public IP addresses
- Private IP addresses
- Credentials
- Secrets
- Telegram bot tokens
- Database passwords
- API keys
- Internal URLs
- Firewall rule details that expose sensitive topology
