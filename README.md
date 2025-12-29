# Ansible Prometheus Grafana Monitoring (RHEL)

Automated deployment of a **production-style monitoring stack** using **Ansible** on **Red Hat Enterprise Linux (RHEL)**.  
The project follows **DevOps best practices** for automation, observability, and infrastructure operations.

---

## 📖 Overview
This repository demonstrates how to deploy and operate a **complete monitoring solution** using Ansible with a focus on:
- Infrastructure as Code (IaC)
- Repeatable and idempotent automation
- Real-world DevOps and SOC monitoring practices

### Stack Components
- **Prometheus** – Metrics collection and scraping
- **Node Exporter** – Host-level system metrics
- **Grafana** – Visualization and dashboards
- **Alerting foundation** – Ready for Alertmanager integration

---

## 🏗️ Architecture

The environment is designed with **clear role separation** and **least-privilege principles**.

### Nodes
- **Control Node**
  - Ansible Master
  - Orchestrates configuration and deployment
  - Excluded from monitoring targets (best practice)

- **Prometheus Server**
  - Central metrics collection
  - Pull-based scraping from Node Exporter endpoints

- **Grafana Server**
  - Dashboards and visualization
  - Uses Prometheus as a data source

- **Node Exporter Nodes**
  - Monitored RHEL servers
  - Provide CPU, memory, disk, and network metrics

---

## 🛠️ Technologies

- Ansible
- Prometheus
- Grafana
- Node Exporter
- Red Hat Enterprise Linux (RHEL)
- systemd
- firewalld
- Git & GitHub

---

## 📁 Project Structure

ansible-prometheus-grafana-monitoring/

├── inventory/

│   └── hosts.ini

├── roles/

│   ├── prometheus/

│   ├── grafana/

│   └── node_exporter/

├── site.yml

└── README.md
---

<img width="1920" height="1080" alt="Screenshot (316)" src="https://github.com/user-attachments/assets/ffbb98c5-3237-41e7-a51d-2cbe84cbc129" />
<img width="1920" height="1080" alt="Screenshot (315)" src="https://github.com/user-attachments/assets/be310124-d0aa-4330-bedc-e7c9f3824bc2" />
<img width="1920" height="1080" alt="Screenshot (314)" src="https://github.com/user-attachments/assets/fe7624ea-76dc-4671-9d03-405e6f6b83fa" />
<img width="1920" height="1080" alt="Screenshot (313)" src="https://github.com/user-attachments/assets/530e06a6-24c6-4b39-84c3-ee8b1eec60c1" />
<img width="1920" height="1080" alt="Screenshot (312)" src="https://github.com/user-attachments/assets/2aa97d0b-326e-4a78-9728-5fbc9100ac2d" />
<img width="1920" height="1080" alt="Screenshot (311)" src="https://github.com/user-attachments/assets/f8d67d70-d477-440d-ad40-1de55756c729" />
<img width="1920" height="1080" alt="Screenshot (310)" src="https://github.com/user-attachments/assets/38c2410e-978b-45b7-8427-ef0fd515746c" />
<img width="1920" height="1080" alt="Screenshot (320)" src="https://github.com/user-attachments/assets/b99f58fd-f7fb-4f96-82b9-3f5dad51c410" />
<img width="1920" height="1080" alt="Screenshot (319)" src="https://github.com/user-attachments/assets/faa3bd88-b5f2-4c7e-8a3b-6533cd84d22b" />

