## Visualizing Threat Data: Enhancing Threat Intelligence Platforms
## Project Overview

This project is our final year cybersecurity capstone, focused on visualizing and analyzing cyber threat data to enhance threat intelligence. We leveraged OpenCTI as the foundation but extended it significantly by:

Creating custom visual dashboards for threat trends, malware campaigns, and attacker activity.

Configuring and integrating multiple connectors for automated ingestion from STIX files, CSV/TXT datasets, AlienVault, and internal threat reports.

Implementing Dockerized multi-service orchestration, including Redis, Elasticsearch, RabbitMQ, MinIO, and OpenCTI workers, to handle scalable and real-time data processing.

Automating alerts and anomaly detection workflows to highlight suspicious activity.

This project demonstrates our hands-on experience in deploying, configuring, and extending real-world threat intelligence platforms and our understanding of the end-to-end cybersecurity data pipeline.

## Key Contributions

Custom Visualizations: Designed dashboards that highlight emerging threats, attack patterns, and high-risk indicators.

Connector Management: Configured, monitored, and automated data ingestion from multiple sources, including STIX files, CSV, TXT, AlienVault, and internal datasets.

Data Processing Pipelines: Implemented scalable worker and queue processing to analyze, enrich, and correlate threat data in real time.

System Orchestration: Built a Docker Compose setup with multiple integrated services ensuring reliability, health checks, and automated restarts.

Reporting & Exporting: Added functionality to export threat intelligence in CSV, TXT, and STIX formats for further analysis.

## Features

Aggregated Threat Intelligence: Collects data from multiple sources and standardizes it for analysis.

Interactive Dashboards: Custom charts and visualizations for malware campaigns, threat actors, and indicators.

Real-Time Monitoring: Detects new threats as they appear using automated ingestion and worker pipelines.

Anomaly Detection: Highlights unusual patterns or spikes in threat activity.

Scalable Architecture: Supports replication of workers and connectors for high-throughput environments.

Secure & Configurable: Fully configurable via environment variables and secure access keys.

## Installation & Usage

Clone the repository:

git clone https://github.com/yourusername/threat-visualization.git
cd threat-visualization


Configure environment variables in .env for MinIO, RabbitMQ, OpenCTI, SMTP, and connectors.

Start the platform:

docker-compose up -d
