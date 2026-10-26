# Hi, I'm Noth1ng 👋

**DevOps / Site Reliability Engineer** who builds and runs production infrastructure: large-scale, high-availability systems serving real users, where
every minute of downtime has a cost.

## 📜 The Validator Oath
> I solemnly swear that:
> - My node will sign blocks even when I'm asleep. **Especially** when I'm asleep.
> - I will read the installer before `curl | bash`. Yes, the whole thing.
> - I will never, ever, call `pow_status` on a running node again. *(We don't talk about October 5th.)*
> - Mandatory upgrades will be applied before the hard fork, not 35 hours after it.
Now applying the same discipline to blockchain: running testnet validators and nodes
the way production should be run, with observability, automation, hardening and postmortems.

## 🔥 Production engineering
- Designed, built and operated **large-scale production platforms**:
  Handling >100 services | 20 nodes | 5 cluster, 4K CCU | >200 VMs
- **High availability by design:** multi-node clusters, load balancing, failover,
  zero-downtime deployments, rolling upgrades with automated rollback.
- **Infrastructure as Code:** reproducible environments with Ansible / Terraform / CI/CD.
- **Observability:** metrics, logs and alerting across the stack; on-call with
  SLO-driven alerts instead of noise.
- **Incident response:** led incident handling end to end, from detection and mitigation to
  blameless postmortems and root-cause fixes that stop the class of failure from recurring.
- **Security hardening:** least privilege, network segmentation, firewall-as-code,
  secrets management, patching discipline.

## 🛰️ Node operations
| Network | Role | Status |
|---|---|---|
| Asentum (testnet) | Validator | 🟢 Active since Oct 2026 |
| Logos (testnet v0.3) | Full node + PoW mining | 🟢 Active since Oct 2026 |
| GenLayer | Validator applicant | 🟡 Waitlist |

**Production practices applied to every node**
- **Observability first:** self-built monitoring platform (FastAPI + PostgreSQL + React) and with Monitoring stack: Prometheus+Grafana. Logging Stack with ELK.
  Nodes push health reports every 5 min over pinned-cert HTTPS; Telegram alerts on block stall,
  height lag, closed ports, RAM/disk pressure, missed reports.
- **Upgrade discipline:** project announcements (X / GitHub / docs) auto-classified by LLM;
  mandatory upgrades keep alerting until done, then a post-upgrade checklist
  (key checksum, sandbox, firewall).
- **Self-healing:** bounded-restart watchdogs for crashed modules and stalled sync;
  cgroup limits so one leaking node can't take down its neighbours.
- **Postmortems:** every incident is written up and fixed at the root cause.

## ⚔ Stack
| | |
|---|---|
| **🖥️ OS & Virtualization** | ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black) ![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=flat-square&logo=ubuntu&logoColor=white) ![Windows](https://img.shields.io/badge/Windows_Server-0078D4?style=flat-square&logo=windows&logoColor=white) ![VMware](https://img.shields.io/badge/VMware_vSphere-607078?style=flat-square&logo=vmware&logoColor=white) ![Proxmox](https://img.shields.io/badge/Proxmox-E57000?style=flat-square&logo=proxmox&logoColor=white) ![systemd](https://img.shields.io/badge/systemd-30D475?style=flat-square&logo=linux&logoColor=black) |
| **📦 Containers & Orchestration** | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white) |
| **⚙️ Automation & CI/CD** | ![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white) ![GitLab](https://img.shields.io/badge/GitLab_CI%2FCD-FC6D26?style=flat-square&logo=gitlab&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white) |
| **📈 Observability** | ![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=flat-square&logo=elasticsearch&logoColor=white) ![Logstash](https://img.shields.io/badge/Logstash-005571?style=flat-square&logo=logstash&logoColor=white) ![Kibana](https://img.shields.io/badge/Kibana-005571?style=flat-square&logo=kibana&logoColor=white) ![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white) ![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white) ![Telegram](https://img.shields.io/badge/Telegram_Alerts-26A5E4?style=flat-square&logo=telegram&logoColor=white) |
| **🌐 Networking** | ![TCP/IP](https://img.shields.io/badge/TCP%2FIP-0A66C2?style=flat-square&logo=cloudflare&logoColor=white) ![Routing & Switching](https://img.shields.io/badge/Routing_%26_Switching-1BA0D7?style=flat-square&logo=cisco&logoColor=white) ![VLAN](https://img.shields.io/badge/VLAN-segmentation-6A5ACD?style=flat-square) ![VPN](https://img.shields.io/badge/VPN-site--to--site-2E8B57?style=flat-square&logo=wireguard&logoColor=white) ![DNS](https://img.shields.io/badge/DNS%20%2F%20LB-F38020?style=flat-square&logo=nginx&logoColor=white) |
| **🔐 Security** | ![Fortinet](https://img.shields.io/badge/FortiGate-EE3124?style=flat-square&logo=fortinet&logoColor=white) ![Firewall](https://img.shields.io/badge/Firewall-default--deny-critical?style=flat-square&logo=letsencrypt&logoColor=white) ![SSH](https://img.shields.io/badge/SSH-key--only-black?style=flat-square&logo=openssh&logoColor=white) |
| **🧑‍💻 Code & Data** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) |
| **⛓️ Blockchain Ops** | ![Validator](https://img.shields.io/badge/Validator-Asentum-8A2BE2?style=flat-square) ![Node](https://img.shields.io/badge/Node-Logos-1E1E1E?style=flat-square) ![GenLayer](https://img.shields.io/badge/GenLayer-waitlist-F5A623?style=flat-square) |
