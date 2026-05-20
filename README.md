# Sysfix — Linux Diagnostics & AI-Powered Repairs

**Professional Linux system diagnostics, AI-powered repairs, security auditing, and more — powered by Fyxa AI.**

Sysfix is an all-in-one Linux health tool. It scans your system for problems — memory leaks, overheating, disk pressure, failed services — and uses a local AI (Fyxa) to understand what's wrong and help you fix it. Fyxa remembers your hardware and past solutions in a persistent local brain, getting smarter over time.

---

## Latest Release: **v1.2.0**

May 2026. A major reliability and UX release. Closed-source build — only the application is distributed; source is not included.

### What's new

- **Risk-aligned Pro gating** — free users can now apply *safe* one-click fixes (cache clears, DNS flush, common maintenance). Only risky/system-level changes and batch automation remain Pro.
- **New: System Health** screen — Self-Diagnostic + Performance Benchmark + Disk Cleanup in one place. CLI: `sysfix doctor`, `sysfix benchmark`, `sysfix cleanup`.
- **New: Battery Health** card on the dashboard (laptops; auto-hidden on desktops). Real capacity wear, cycle count, live draw, time-left estimate.
- **New: Crash recovery banner** — on the next launch after a crash, a dismissible banner lets you view/copy the report instead of relaunching blind.
- **Responsive dashboard** — flows cleanly at 1 / 2 / 3 / 4 columns by window width.
- Plus dozens of fixes: font crash on boot, RAM-Turbo control loss on refresh, dead debug-tool action buttons, broken auto-rollback safety net, stale screen data on navigation, and more.

> **Pro activation:** v1.2.0 ships with Pro activation cleanly disabled ("coming soon"). The free tier is fully functional — diagnostics, safe one-click fixes, monitoring, theming. Pro unlock arrives in a follow-up release.

### Install

Download the assets from the [v1.2.0 release page](https://github.com/useofscript/Sysfix-Releases/releases/tag/v1.2.0), then:

#### Fedora / RHEL / openSUSE (RPM)

```bash
sudo dnf install ./sysfix-ai-1.2.0-1.fc44.noarch.rpm
```

#### Debian / Ubuntu / Linux Mint (DEB)

```bash
sudo apt install ./sysfix-ai_1.2.0-1_all.deb
```

#### Verify the download

```bash
sha256sum -c SHA256SUMS.txt
```

### Launch

```bash
sysfix              # GUI (default)
sysfix doctor       # self-diagnostic — verify Sysfix can do its job
sysfix benchmark    # CPU / memory / disk score with before/after delta
sysfix scan         # run diagnostics from the terminal
sysfix history      # see what Sysfix has changed
sysfix rollback     # restore an earlier snapshot
sysfix --help       # full command list
```

---

## Free vs Pro

| Feature                          | Free          | Pro ⭐                |
|----------------------------------|---------------|-----------------------|
| Diagnostics & live monitors      | ✓             | ✓                     |
| Fyxa AI chat                     | ✓             | ✓                     |
| Repair actions                   | Safe fixes    | All · automated       |
| Autonomous repair loop           | —             | ✓                     |
| Omni-Turbo & RAM-Turbo (actions) | —             | ✓                     |
| Turbo/zRAM status display        | ✓ visible     | ✓ + can apply         |
| Debug tools (7)                  | View only     | Full control          |
| Background daemon                | —             | ✓                     |
| Seasonal & custom themes         | 6 themes      | Unlimited             |
| Price                            | Free          | $5 one-time           |

---

## Security & integrity

- Packages ship **without source code** — only the compiled application is distributed.
- Every shipped file is SHA-256 hashed; Sysfix re-verifies its own integrity at every launch.
- Verify the package checksum against `SHA256SUMS.txt` before installing.
- Set `SYSFIX_STRICT_INTEGRITY=1` if you want Sysfix to refuse to start on any integrity mismatch.

---

## Older releases

- [v1.1.0](https://github.com/useofscript/Sysfix-Releases/releases/tag/v1.1.0) — March 2026
- [v1.0.0](https://github.com/useofscript/Sysfix-Releases/releases/tag/v1.0.0) — March 2026 (first stable)

## License

Proprietary. See [LICENSE](LICENSE) — source-available for review only; redistribution and reverse-engineering are not permitted.
