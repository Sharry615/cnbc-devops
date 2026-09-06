# Compute Engine

## Analytics VM

The CNBC environment contains a Compute Engine VM:

- Name: `cnbc-analytics`
- Zone: `europe-west3-a`

The supplied screenshot does not establish the exact application/workload running on this VM.

## Monitoring

The VM is monitored through Zabbix for infrastructure health, including:

- CPU utilization
- Memory utilization
- Disk utilization
- Network activity
- Availability / host health

Zabbix alerts are integrated with Telegram.
