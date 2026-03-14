# Sysfix — Linux Diagnostics & AI-Powered Repairs

**Professional Linux system diagnostics, AI-powered repairs, security auditing, and more — powered by Fyxa AI.**

Sysfix is an all-in-one Linux health tool. It scans your system for problems — memory leaks, overheating, disk pressure, failed services — and uses a local AI (Fyxa) to understand what's wrong and help you fix it. Fyxa remembers your hardware and past solutions in a persistent local brain, getting smarter over time.

---

## Latest Release: v1.1.0

March 2026. Pre-compiled bytecode build (no source code included).

### Install

#### Fedora / RHEL / openSUSE (RPM)

```bash
sudo dnf install ./rpms/sysfix-ai-1.1.0-1.fc43.noarch.rpm
```

#### Debian / Ubuntu / Linux Mint (DEB)

```bash
sudo apt install ./rpms/sysfix-ai_1.1.0-1_all.deb
```

### Launch

```bash
sysfix          # GUI (default)
sysfix gui      # Force GUI
sysfix check    # Run diagnostics (CLI)
sysfix --help   # All commands
```

---

## What's Included (Free)

Everything below works out of the box with no licence key.

- **7-tab GUI** — Dashboard, Quick Fix, Security, Network, Health, AI Chat, Brain
- **Fyxa AI assistant** — local LLM-powered diagnostics via [Ollama](https://ollama.com) (optional install)
- **Diagnostics engine** — CPU, RAM, disk, temperature, audio, BIOS, and motherboard issue detection
- **Fast Sweep** — one-click AI-powered auto-fix with confirmation
- **Deep Dive** — interactive AI troubleshooting session
- **Security auditing** — listening ports, firewall status, failed logins, SUID binaries, rootkit checks, SSH review
- **Network diagnostics** — Wi-Fi info, DNS resolution, traceroute, gateway latency, bandwidth, active connections, public IP
- **System health** — boot time, systemd analysis, failed services, journal errors
- **Malware scanning** — SHA-256 hash checks against MalwareBazaar, ClamAV, YARA rules
- **Persistent brain/memory** — learns your system's hardware, projects, and past fixes
- **Full CLI** — 14+ commands (`sysfix check`, `sysfix security`, `sysfix chat`, `sysfix network`, etc.)
- **5 built-in themes** — Frutiger Aero (default), Light, Dark, Cyberpunk, Glass
- **eBPF Sentinel** — real-time process monitor using BPF Compiler Collection (bcc)
- **Sandbox dry-runs** — test commands in an isolated environment before applying
- **Hardware health score** — 0–100 composite score across thermal, memory, CPU, disk, battery, and fan sensors

---

## Sysfix Pro — Paid Licence ($15 one-time)

A one-time purchase that unlocks premium features. Buy at: [Sysfix Pro on Polar](https://buy.polar.sh/polar_cl_tTB6FDmTJCTv08FdiaawTOA7WN0rxz6Q8RHWA40vu4G)

### What the Pro licence adds

| Feature | Description |
| ------- | ----------- |
| **Agentic Reasoning Engine** | Think-Act-Observe cycle — Fyxa becomes a stateful system architect that can plan multi-step repairs |
| **Hardware Governor** | Automatic CPU governor tuning, GPU clock management (NVIDIA/Intel/AMD), compositor optimisation |
| **RAM Turbo** | Intelligent ZRAM/ZSWAP optimisation, kernel memory tuner, automatic memory pressure relief |
| **Universal Brain (4-pillar engine)** | Distro-agnostic AI brain with live hardware telemetry, anomaly detection, and GGUF model fallback |
| **Sentinel AV** | Kernel-level behavioural antivirus — hooks execve, tcp_v4_connect, and openat syscalls via eBPF |
| **Sentinel Bridge** | Pure-Python security bridge — exposes Sentinel data to the AI without requiring root or python3-bcc |
| **Micro-VM Sandbox** | Run risky commands in a Firecracker micro-VM (~150 ms boot, fully isolated from host) |
| **NPU Offloading** | Detect and use Intel Core Ultra / AMD Ryzen AI NPUs for AI inference acceleration |
| **PRO Discord role** | Access to the #pro channel on the Sysfix Discord server |
| **Priority support** | Direct support from the developer |

### What the Pro licence does NOT include

Sysfix Pro is a **Linux system diagnostics and repair tool**. It does not include, promote, or facilitate:

- Third-party content downloaders or media rippers
- DRM circumvention or copy-protection bypass tools
- Piracy, scraping, or data-harvesting utilities
- Proxy, VPN, or anonymisation services

The Polar checkout is exclusively for the Sysfix Pro diagnostic software licence.

---

## Requirements

- Linux (any distribution — Fedora, Ubuntu, Debian, Arch, openSUSE, etc.)
- Python 3.8+
- `python3-tkinter` / `python3-tk` (for GUI)

**Optional:** Install [Ollama](https://ollama.com) for AI features. Without Ollama, all non-AI features work normally.

---

## Files

| File | Distro |
| ---- | ------ |
| `sysfix-ai-1.1.0-1.fc43.noarch.rpm` | Fedora, RHEL, openSUSE |
| `sysfix-ai_1.1.0-1_all.deb` | Debian, Ubuntu, Linux Mint |
| `SHA256SUMS.txt` | Package checksums |

---

## v1.1.0 Changelog

- Fix asset/mascot loading on installed packages (RPM/DEB) — icons and Fyxa mascot now load correctly
- Agentic reasoning engine with Think-Act-Observe cycle
- 4-pillar architecture: Universal Brain, Hardware Governor, RAM Turbo, License Guard
- Local-first AI engine with Ollama + GGUF fallback
- Resolve all Pylance/Pyright type errors
- Fix critical missing import in licence guard module

## Licence

Proprietary — free to use, not for resale. See [LICENSE](LICENSE).
