<p align="center">
  <img src="https://img.shields.io/badge/Claude-Skills-blueviolet?style=for-the-badge&logo=anthropic" alt="Claude Skills">
  <img src="https://img.shields.io/badge/Terminal-Focused-green?style=for-the-badge&logo=gnometerminal" alt="Terminal">
  <img src="https://img.shields.io/badge/License-Apache%202.0-blue?style=for-the-badge" alt="License">
  <img src="https://img.shields.io/badge/Skills-59+-orange?style=for-the-badge" alt="Skills Count">
</p>

<h1 align="center">🖥️ Terminal Skills</h1>

<p align="center">
  <strong>A curated collection of Claude Skills for terminal, server, DevOps, and cloud operations</strong>
</p>

<p align="center">
  <a href="#-features">Features</a> •
  <a href="#-quick-start">Quick Start</a> •
  <a href="#-skill-categories">Categories</a> •
  <a href="#-popular-skills">Popular</a> •
  <a href="#-contributing">Contributing</a>
</p>

<p align="center">
  <a href="./README_CN.md">🇨🇳 中文文档</a>
</p>

---

## 🎯 What is Terminal Skills?

Terminal Skills is a comprehensive collection of [Claude Skills](https://docs.anthropic.com/en/docs/claude-code/skills) designed specifically for terminal-based workflows. Each skill provides Claude with domain-specific knowledge and commands for system administration, DevOps, cloud operations, and more.

**Why use Terminal Skills?**
- 🚀 **Instant expertise** - Claude gains deep knowledge of specific tools and workflows
- 📋 **Battle-tested commands** - Real-world commands with best practices built-in
- 🔧 **Troubleshooting guides** - Common issues and solutions included
- 🎓 **Learning resource** - Great for both beginners and experienced engineers

## ✨ Features

| Category | Description | Skills |
|----------|-------------|--------|
| 🐧 **Linux** | System administration, file operations, process management, shell scripting | 6 |
| 🖧 **Server** | Nginx, Apache, SSH, Systemd, Cron, log analysis | 6 |
| 🗄️ **Database** | MySQL, PostgreSQL, MongoDB, Redis, Elasticsearch, SQL optimization | 6 |
| ☸️ **Kubernetes** | kubectl, deployments, services, Helm, troubleshooting | 7 |
| 🐳 **Docker** | Container operations, images, Compose, networking, Dockerfile | 5 |
| ☁️ **Cloud CLI** | AWS CLI, Azure CLI, Google Cloud, Alibaba Cloud | 4 |
| 🔧 **DevOps** | Git advanced, Ansible, Terraform, CI/CD, monitoring | 5 |
| 🌐 **Network** | TCP/IP, DNS, VPN, proxy, load balancer, traffic analysis | 6 |
| 💾 **Backup** | rsync, tar, snapshots, cloud backup, disaster recovery | 6 |
| 🔒 **Security** | Firewall, SSL/TLS, audit, system hardening | 4 |
| 📊 **Performance** | Benchmarking, profiling, tuning, troubleshooting | 4 |

**Total: 59 Skills**

## 🚀 Quick Start

### Installation

```bash
git clone https://github.com/your-username/terminal-skills.git
cd terminal-skills
```

### Usage with Claude Code

1. Copy the desired skill folder to your Claude skills directory:
   ```bash
   # Example: Add kubectl-basics skill
   cp -r kubernetes/kubectl-basics ~/.claude/skills/
   ```

2. Or reference skills directly in your project:
   ```bash
   # Add to your project's .claude/skills directory
   cp -r linux/file-operations ./your-project/.claude/skills/
   ```

3. Claude will automatically load and use the skill when relevant

### Skill Structure

Each skill follows a consistent structure:

```
skill-name/
├── SKILL.md          # Main skill file with instructions and commands
├── examples/         # Usage examples (optional)
├── scripts/          # Helper scripts (optional)
└── resources/        # Additional references (optional)
```

### SKILL.md Format

```yaml
---
name: skill-name
description: Brief description
version: 1.0.0
author: contributor-name
tags: [tag1, tag2, tag3]
---

# Skill Title

## Overview
What this skill does and when to use it.

## Core Commands
Essential commands with explanations.

## Common Scenarios
Real-world use cases with step-by-step guides.

## Troubleshooting
Common issues and solutions.
```

## 📂 Skill Categories

### 🐧 Linux System Administration

| Skill | Description |
|-------|-------------|
| [file-operations](./linux/file-operations) | File and directory operations, find, permissions |
| [process-management](./linux/process-management) | Process monitoring, signals, job control |
| [user-permissions](./linux/user-permissions) | User management, sudo, ACL |
| [network-tools](./linux/network-tools) | Network diagnostics, netstat, ss, ip |
| [system-admin](./linux/system-admin) | System monitoring, resource management |
| [shell-scripting](./linux/shell-scripting) | Bash scripting, automation |

### 🖧 Server Operations

| Skill | Description |
|-------|-------------|
| [nginx](./server/nginx) | Nginx configuration, virtual hosts, SSL |
| [apache](./server/apache) | Apache httpd configuration and management |
| [ssh](./server/ssh) | SSH configuration, keys, tunneling |
| [systemd](./server/systemd) | Service management, units, journalctl |
| [cron](./server/cron) | Scheduled tasks, crontab |
| [log-analysis](./server/log-analysis) | Log parsing, analysis, monitoring |

### 🗄️ Database Management

| Skill | Description |
|-------|-------------|
| [mysql](./database/mysql) | MySQL administration, queries, backup |
| [postgresql](./database/postgresql) | PostgreSQL management, psql, replication |
| [mongodb](./database/mongodb) | MongoDB operations, aggregation, sharding |
| [redis](./database/redis) | Redis commands, persistence, clustering |
| [elasticsearch](./database/elasticsearch) | Elasticsearch queries, indices, cluster |
| [sql-optimization](./database/sql-optimization) | Query optimization, indexing, explain |

### ☸️ Kubernetes

| Skill | Description |
|-------|-------------|
| [kubectl-basics](./kubernetes/kubectl-basics) | Essential kubectl commands |
| [pod-management](./kubernetes/pod-management) | Pod lifecycle, debugging |
| [deployment](./kubernetes/deployment) | Deployments, rollouts, scaling |
| [service-ingress](./kubernetes/service-ingress) | Services, Ingress, networking |
| [configmap-secret](./kubernetes/configmap-secret) | Configuration management |
| [helm](./kubernetes/helm) | Helm charts, releases |
| [troubleshooting](./kubernetes/troubleshooting) | K8s debugging and diagnostics |

### 🐳 Docker

| Skill | Description |
|-------|-------------|
| [container-ops](./docker/container-ops) | Container lifecycle management |
| [image-management](./docker/image-management) | Image building, tagging, registry |
| [dockerfile](./docker/dockerfile) | Dockerfile best practices |
| [compose](./docker/compose) | Docker Compose multi-container apps |
| [networking](./docker/networking) | Docker networking, bridges, overlay |

### ☁️ Cloud CLI

| Skill | Description |
|-------|-------------|
| [aws-cli](./cloud-cli/aws-cli) | AWS CLI for EC2, S3, IAM, etc. |
| [azure-cli](./cloud-cli/azure-cli) | Azure CLI operations |
| [gcloud](./cloud-cli/gcloud) | Google Cloud CLI |
| [aliyun-cli](./cloud-cli/aliyun-cli) | Alibaba Cloud CLI |

### 🔧 DevOps Tools

| Skill | Description |
|-------|-------------|
| [git-advanced](./devops/git-advanced) | Advanced Git workflows, rebasing |
| [ansible](./devops/ansible) | Ansible playbooks, inventory |
| [terraform](./devops/terraform) | Infrastructure as Code |
| [ci-cd](./devops/ci-cd) | CI/CD pipelines, GitHub Actions |
| [monitoring](./devops/monitoring) | Prometheus, Grafana, alerting |

### 🌐 Network

| Skill | Description |
|-------|-------------|
| [tcp-ip](./network/tcp-ip) | TCP/IP fundamentals, troubleshooting |
| [dns](./network/dns) | DNS configuration, dig, nslookup |
| [vpn](./network/vpn) | VPN setup and management |
| [proxy](./network/proxy) | Proxy servers, reverse proxy |
| [load-balancer](./network/load-balancer) | Load balancing strategies |
| [traffic-analysis](./network/traffic-analysis) | tcpdump, Wireshark, packet analysis |

### 💾 Backup & Recovery

| Skill | Description |
|-------|-------------|
| [rsync](./backup-recovery/rsync) | rsync for file synchronization |
| [tar-compression](./backup-recovery/tar-compression) | Archive and compression |
| [snapshot](./backup-recovery/snapshot) | Filesystem snapshots |
| [cloud-backup](./backup-recovery/cloud-backup) | Cloud backup strategies |
| [backup-strategy](./backup-recovery/backup-strategy) | Backup planning and policies |
| [disaster-recovery](./backup-recovery/disaster-recovery) | DR planning and execution |

### 🔒 Security

| Skill | Description |
|-------|-------------|
| [firewall](./security/firewall) | iptables, firewalld, ufw |
| [ssl-tls](./security/ssl-tls) | SSL/TLS certificates, Let's Encrypt |
| [audit](./security/audit) | Security auditing, compliance |
| [hardening](./security/hardening) | System hardening best practices |

### 📊 Performance

| Skill | Description |
|-------|-------------|
| [benchmarking](./performance/benchmarking) | Performance benchmarking tools |
| [profiling](./performance/profiling) | Application profiling |
| [tuning](./performance/tuning) | System and application tuning |
| [troubleshooting](./performance/troubleshooting) | Performance issue diagnosis |

## 🎯 Popular Skills

### kubectl-basics
```bash
# Quick pod status check
kubectl get pods -o wide

# Enter container for debugging
kubectl exec -it pod-name -- /bin/bash

# View recent logs
kubectl logs pod-name --tail=100
```

### mysql
```bash
# Database backup
mysqldump -u root -p database > backup.sql

# Check slow queries
SHOW VARIABLES LIKE 'slow_query%';

# Restore database
mysql -u root -p database < backup.sql
```

### rsync
```bash
# Incremental backup with progress
rsync -avzP --delete source/ dest/

# Remote sync over SSH
rsync -avz -e ssh /local/path user@remote:/remote/path
```

### docker container-ops
```bash
# Run container with resource limits
docker run -d --name app --memory=512m --cpus=1 nginx

# View container logs in real-time
docker logs -f container_name

# Enter running container
docker exec -it container_name /bin/bash
```

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guide](./CONTRIBUTING.md) for details.

**Quick contribution steps:**

1. Fork the repository
2. Create a new skill folder under the appropriate category
3. Write your `SKILL.md` following the template
4. Submit a Pull Request

**What makes a good skill?**
- ✅ Clear, tested commands
- ✅ Real-world scenarios
- ✅ Troubleshooting section
- ✅ Proper frontmatter metadata

## 📄 License

This project is licensed under the [Apache License 2.0](./LICENSE).

## 🔗 Related Resources

- [Claude Skills Documentation](https://docs.anthropic.com/en/docs/claude-code/skills)
- [awesome-claude-skills](https://github.com/travisvn/awesome-claude-skills) - Curated list of Claude Skills
- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) - Claude Code documentation

## 🌟 Star History

If you find this project helpful, please consider giving it a ⭐ star!

---

<p align="center">
  Made with ❤️ for the DevOps community
</p>
