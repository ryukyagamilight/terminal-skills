# terminal-skills

A collection of **Claude Skills** for terminal-centric workflows: **servers / Linux / SSH bastion / Docker / Kubernetes / Databases**.

Each skill is a self-contained folder with a required `SKILL.md` (YAML frontmatter + instructions), plus optional `scripts/`, `references/`, `assets/`. This follows the common Claude Skills packaging pattern. 

## What’s inside

### Linux / Server
- `linux-basics` — Common Linux commands & quick reference.
- `linux-troubleshooting` — CPU/memory/disk/IO triage playbook + scripts.
- `systemd-ops` — `systemctl` / `journalctl` workflows.
- `log-investigation` — Grep/ripgrep/jq log analysis, timeline building, secret redaction.
- `network-diagnostics` — DNS/TCP/routing/curl/tcpdump playbooks.

### SSH / Bastion
- `ssh-bastion-ops` — SSH config patterns, jump host, tunneling, port forwarding.

### Containers
- `docker-ops` — Container debugging (resources, logs, networking).

### Kubernetes
- `k8s-basics` — kubectl recipes, JSONPath/go-template, patch/rollout patterns.
- `k8s-troubleshooting` — Pod/Service/Ingress/DNS/scheduling/networking incident playbooks.
- `helm-release-ops` — Helm install/upgrade/rollback and chart debugging.

### Databases
- `database-mysql` — Slow query/locks/replication/backups.
- `database-postgres` — EXPLAIN/index/locks/vacuum/backups.
- `database-redis` — Hotkey/bigkey/memory/replication/cluster.
- `sql-reviewer` — SQL review & migration risk checklist.

### Resilience & Security
- `backup-restore` — Backup strategy, restore drill, RPO/RTO validation.
- `security-hardening` — Baseline hardening & audit reminders.

---

## Install / Use

### Option A: Claude Code (local skills folder)
Copy one or more skill folders into your Claude skills directory (example path):

```bash
mkdir -p ~/.claude/skills
cp -r ./terminal-skills/k8s-troubleshooting ~/.claude/skills/
cp -r ./terminal-skills/linux-troubleshooting ~/.claude/skills/
