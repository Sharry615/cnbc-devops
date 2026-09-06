# Grafana, Zabbix & Telegram Monitoring

CNBC follows the common centralized monitoring model used across the DevOps portfolio.

## Grafana

Grafana is used for:

- Application logs
- Application/platform metrics
- Dashboards
- Operational visualization

## Zabbix

Zabbix is used primarily for infrastructure and VM monitoring:

- CPU
- Memory
- Disk
- Network
- Host availability
- Infrastructure health

## Telegram

Telegram is the common alert notification channel.

```text
                GRAFANA
             Logs + Metrics
                  |
                  v
               TELEGRAM
                  ^
                  |
                ZABBIX
       CPU / Memory / Disk / VM
```

Both Grafana and Zabbix can generate alerts that are delivered through Telegram.

## Portfolio-Wide Model

```text
PTI | Masti | SMS | CNBC | IKOMG | Art of Living
                         |
              +----------+----------+
              |                     |
            Grafana               Zabbix
         Logs + Metrics       VM / Infrastructure
              |                     |
              +----------+----------+
                         |
                      Telegram
                       Alerts
```
