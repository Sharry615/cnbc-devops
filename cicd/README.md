# CI/CD

The supplied CNBC screenshots establish the deployed GCP resources but do not identify the CI/CD platform.

Therefore this repository intentionally does not claim Jenkins, Cloud Build, GitHub Actions, Bitbucket Pipelines or another CI/CD product without confirmation.

## Expected Deployment Flow

Once the actual CI/CD platform is confirmed, the deployment flow can be documented as:

```text
Source Repository
       |
       v
CI/CD Pipeline
       |
       v
Build / Test
       |
       v
Container Image
       |
       v
Artifact Registry
       |
       v
Cloud Run
```

This is a documentation placeholder, not a claim that every step above is currently implemented exactly this way.
