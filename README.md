# Pi Cluster (SCRAPED IDEA)

A 6-node Raspberry Pi cluster running K3s (lightweight Kubernetes) with Grafana monitoring.

## Hardware
- 1x Raspberry Pi 5 (master node)
- 5x Raspberry Pi Zero 2W (worker nodes)
- Network switch for local communication

## Stack
- **K3s** — lightweight Kubernetes for node orchestration
- **Prometheus** — metrics collection from all nodes
- **Grafana** — live dashboard for cluster monitoring

## Architecture
```
[Laptop] ──── [Switch] ──── [Pi 5 / master]
                    │──── [Zero 2W / node-01]
                    │──── [Zero 2W / node-02]
                    │──── [Zero 2W / node-03]
                    │──── [Zero 2W / node-04]
                    └──── [Zero 2W / node-05]
```

## Status
🔧 In progress — setting up K3s and Grafana

## Roadmap
- [ ] Flash and configure all nodes
- [ ] K3s master setup on Pi 5
- [ ] Join worker nodes to cluster
- [ ] Deploy Prometheus + Grafana
- [ ] Document setup guide
