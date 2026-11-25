# Windows Network Observability Stack

Real-time Windows network interface monitoring pipeline using **windows_exporter**, **Prometheus**, and **Grafana**.

## Architecture

`windows_exporter` (`:9182`) -> `Prometheus` (`:9090`) -> `Grafana` (`:3001`)

## Quick Start

1. Start `windows_exporter.exe --collectors.enabled="net"`
2. Start `prometheus.exe --config.file=prometheus.yml`
3. Start `grafana-server.exe` and import `dashboards/windows-network.json`.
