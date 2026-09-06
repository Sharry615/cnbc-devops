# Deployment Overview

CNBC has separate staging and production environments.

## Staging

Changes are validated in the staging environment before production rollout.

## Production

Production contains independently deployed Cloud Run services for the platform workloads.

## Deployment Safety

Recommended practices:

1. Validate application changes in staging.
2. Run automated tests and security checks.
3. Build immutable container images.
4. Deploy a new Cloud Run revision.
5. Validate health and application behavior.
6. Monitor Grafana and Zabbix.
7. Use controlled rollout/rollback procedures.

The exact existing pipeline implementation is not specified by the supplied screenshots.
