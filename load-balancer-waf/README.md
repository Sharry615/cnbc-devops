# Load Balancing & WAF

The CNBC project uses external Application Load Balancers.

The supplied console view shows multiple load balancers with HTTPS and HTTP frontends and backend configurations containing:

- Cloud Run backend services
- Backend buckets
- Redirect configurations

## WAF

WAF protection is used for the platform.

The portfolio documentation keeps the WAF layer generic until the exact Cloud Armor policy configuration is separately confirmed.

## Security Model

```text
Client
  |
  v
HTTPS Load Balancer
  |
  v
WAF
  |
  +---- Cloud Run
  |
  +---- Backend Bucket
```

Sensitive forwarding rules, IP addresses, certificates and policy rule details should not be published.
