# Docker Observability Toolkit

Welcome to **Docker Observability Toolkit**! 🎓  
This repository is designed as a **pedagogical tool** for exploring modern observability solutions with Docker. Learn by doing: logs, metrics, and monitoring all in one place.

## Project Overview

This repository contains ready-to-use Docker Compose setups for popular observability tools:

- **ELK Stack + Filebeat**
  - Centralized logging with Elasticsearch, Logstash, and Kibana
  - Filebeat for log shipping

- **Grafana + Loki + Promtail**
  - Metrics and log visualization
  - Prometheus integration for monitoring

- **Zabbix**
  - Classic IT monitoring and alerting

## Directory Structure

```text
├── elk
│ ├── docker-compose.yml
│ ├── filebeat
│ │ └── filebeat.yml
│ ├── logstash
│ │ └── pipeline
│ │ └── logstash.conf
│ └── logstash
│ └── pipeline
├── grafana-loki
│ ├── docker-compose.yml
│ ├── prometheus.yml
│ └── promtail-config.yml
└── zabbix
└── docker-compose.yml
```


## Getting Started

1. Clone the repository:

```bash
git clone git@github.com:Jerom-e/docker-observability-stack.git
cd docker-observability-tools
```


2. Choose the stack you want to run:
```bash
cd elk        # or grafana-loki / zabbix
docker-compose up -d
```

3. Access the services :

ELK: Kibana at http://localhost:5601

Grafana: http://localhost:3000

Zabbix: http://localhost:8080

## Purpose

This project is meant for:

DevOps learning and experimentation

HR-friendly internal training

Quick demo environments for logs, metrics, and monitoring

## Contributing

Contributions are welcome! Feel free to suggest improvements, add monitoring tools, or provide better configuration examples.
