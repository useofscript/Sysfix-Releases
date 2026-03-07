# Sysfix AI — Releases

Pre-built RPM packages for **Sysfix AI**, a professional Linux diagnostics tool with AI-powered fixes.

## Latest Release: v1.0.0

First stable release — March 2026.

### Install

```bash
sudo dnf install ./rpms/sysfix-ai-1.0.0-1.fc43.noarch.rpm
```

### What's Included

- **7-tab GUI** — Dashboard, Quick Fix, Security, Network, Health, AI Chat, Brain
- **Fyxa AI assistant** — local LLM-powered via Ollama (optional)
- **Security auditing** — rootkit checks, firewall, ClamAV integration
- **Network diagnostics** — Wi-Fi, DNS, traceroute, bandwidth, connections
- **System health** — boot time, systemd analysis, SMART disk monitoring
- **Persistent brain/memory** — learns your system over time
- **Full CLI** — 14+ commands (`sysfix check`, `sysfix security`, `sysfix chat`, etc.)
- **4 built-in themes** — Frutiger Aero, Light, Dark, Cyberpunk

### Requirements

- Fedora 40+ (or compatible RPM-based distro)
- Python 3.8+
- `python3-tkinter` (for GUI)

Optional: Install [Ollama](https://ollama.com) for AI features.

### Launch

```bash
sysfix          # GUI (default)
sysfix gui      # Force GUI
sysfix check    # Run diagnostics (CLI)
sysfix --help   # All commands
```

## Files

| File | Description |
|------|-------------|
| `rpms/sysfix-ai-1.0.0-1.fc43.noarch.rpm` | Binary RPM (noarch) |
| `rpms/sysfix-ai-1.0.0-1.fc43.src.rpm` | Source RPM |

## License

Proprietary — free to use, not for resale. See [LICENSE](LICENSE).
