#  Monitoring Stack with Prometheus, Grafana & Loki

This project sets up a complete observability stack using Prometheus, Grafana, and Loki for monitoring, logging, and visualization in a containerized environment.

It is designed to demonstrate a production-style monitoring setup using Docker Compose, enabling centralized metrics collection, log aggregation, and real-time dashboarding.

---

##  Overview

This stack includes:

- Prometheus → Metrics collection and monitoring
- Grafana → Visualization and dashboards
- Loki → Log aggregation system
- Promtail → Log collector for Loki

All services are containerized and orchestrated using Docker Compose for easy setup and deployment.

---

##  Architecture

Application Logs → Promtail → Loki → Grafana
Metrics → Prometheus → Grafana
- Prometheus scrapes metrics from configured targets
- Loki collects and stores logs
- Grafana connects to both Prometheus and Loki for visualization

---

##  Project Structure

.
├── docker-compose.yml
├── prometheus/
│ └── prometheus.yml
├── grafana/
│ └── datasource.yml
├── loki/
│ ├── loki-config.yml
│ └── promtail-config.yml


---

##  Setup & Installation
### Prerequisites

- Docker
- Docker Compose

### Run the stack

```bash
docker-compose up -d
```

### Default Grafana login:
Username: admin
Password: admin

Use Case

This project demonstrates how to:
Build a monitoring system for microservices or cloud-native applications
Implement observability in DevOps workflows
Troubleshoot systems using logs and metrics in one place

