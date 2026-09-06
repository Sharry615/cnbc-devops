# Project Information

## Platform

CNBC digital platform hosted on Google Cloud Platform.

## Environments

| Environment | Region |
|---|---|
| Production | europe-west3 |
| Staging | europe-west3 |

## Production Cloud Run Services

- `cnbc-production-admin-backend`
- `cnbc-production-admin-frontend`
- `cnbc-production-client-frontend`
- `cnbc-production-news`
- `cnbc-production-zagtrader`

A Cloud Run Functions-based service named `telegram-alert` is also visible in the environment.

## Staging Cloud Run Services

- `cnbc-staging-admin-backend`
- `cnbc-staging-admin-frontend`
- `cnbc-staging-client-frontend`
- `cnbc-stage-news`

## Database

Two Cloud SQL instances are visible:

- `cnbc-production` — PostgreSQL 17, Enterprise
- `cnbc-staging` — PostgreSQL 17, Enterprise

## Compute

- `cnbc-analytics` — Compute Engine VM in `europe-west3-a`

## Storage

Application buckets visible include:

- `cnbc-production`
- `cnbc-staging`
- `cnbc-citizen-videostech-cloud`

## Networking

External Application Load Balancers provide HTTPS/HTTP entry points and route traffic to Cloud Run services and backend buckets.

## Security

WAF protection is used. The exact policy/rule configuration is intentionally not documented until separately confirmed.

## CI/CD

The screenshots supplied for this project do not establish the CI/CD platform. The repository therefore does not claim a specific CI/CD product.

## Analytics VM

The exact workload running on `cnbc-analytics` was not established by the supplied screenshots. It is documented as an analytics Compute Engine workload without inventing implementation details.
