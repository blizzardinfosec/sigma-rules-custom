## 🧩 Custom Sigma Rules

This repository contains original Sigma rules I've authored and tuned for real-world detection engineering environments—including endpoints, cloud infrastructure, SaaS platforms, and containerized workloads.

### 📚 Coverage Categories

- 🪟 **Windows** – PowerShell abuse, credential access, LOLBins, suspicious child processes, registry persistence  
- 🐧 **Linux** – Cronjob abuse, rootkit indicators, shell access patterns, container entrypoints  
- 🍎 **macOS** – LaunchAgents, `osascript` clipboard access, TCC abuse, minimal shell launches  
- ☁️ **Cloud** – AWS log-based detections, host volume abuse, initial EKS cluster coverage  
- 🧾 **SaaS** – Okta MFA bypass, Microsoft 365 mailbox manipulation, login anomalies  
- 🐳 **Containers** – Shells in minimal images, `/proc` mount detection, Docker socket abuse  
- ☸️ **Kubernetes** – `kubectl exec`, HostPath volume creation, SA token misuse, RBAC lateral movement  

### 📌 Conventions

- 🧠 Mapped to [MITRE ATT&CK](https://attack.mitre.org/)  
- 🔍 Tuned for **high signal, low noise**  
- 🛠️ Each rule includes:
  - `logsource` (platform/service-specific)
  - `detection` (clear logic blocks)
  - `falsepositives` and `level` fields  
- 📦 Organized by platform (e.g. `/windows/`, `/macos/`, `/linux/`, `/kubernetes/`)  
- 🚧 **Work in progress** — continuously growing library built to be used in production pipelines
