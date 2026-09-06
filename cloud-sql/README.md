# Cloud SQL

Two separate Cloud SQL PostgreSQL 17 instances are visible.

## Production

- Instance: `cnbc-production`
- Engine: PostgreSQL 17
- Edition: Enterprise

## Staging

- Instance: `cnbc-staging`
- Engine: PostgreSQL 17
- Edition: Enterprise

The console shows both private and public IP addresses. Application connectivity mode was not established by the supplied screenshots, so this documentation does not claim a specific connectivity path.

## Operational Practices

Recommended production controls include:

- Automated backups
- Point-in-time recovery where required
- Least-privilege database users
- Private connectivity where architecture permits
- TLS/encrypted connections
- Monitoring and alerting
- Regular restore testing
