# Hey — I'm QuantumCat 🐱

Self-taught cybersecurity & networking. Linux, Python, Wireshark, and a
healthy suspicion of my own network traffic.

![QuantumCat logo](logo-1024.png)

## What I'm building

**[QuantumCat SOC Toolkit](https://quantumcatsoc.gumroad.com/l/quantumcat-soc-toolkit)** —
a beginner-friendly desktop app for watching your own machine:

- **Live connection monitor** — new connections as they happen, LOCAL/EXTERNAL
  tagging, top talkers
- **Port scanner** — threaded, 25 well-known ports, open / closed / filtered
- **Snapshot report** — one click, a timestamped triage report of your machine
- **AI Analyst** — plain-English verdicts on what the tools find, running
  100% locally via Ollama (no cloud, no accounts, no telemetry)

Real installers for Windows (`.msi`, desktop shortcut) and Linux (`.deb` +
portable). Full Python source included. **$12, one-time.**

The build story, embarrassing bugs included:
[I Turned Three Beginner Python Scripts Into a Windows Desktop App](https://dev.to/quantumcatpy/i-turned-three-beginner-python-scripts-into-a-windows-desktop-app-d8o)

## Where it started (May 2026)

Three little scripts I wrote while learning — kept public, flaws and all,
because the flaws were the education:

| Repo | What it does |
| --- | --- |
| [Network-Monitor](https://github.com/Quantumcat-py/Network-Monitor) | Polls `ss -tun`, diffs snapshots, logs new connections, tracks top talkers |
| [Port_scanner](https://github.com/Quantumcat-py/Port_scanner) | ~25-line TCP connect scanner over 11 common ports |
| [Snapshot-Report](https://github.com/Quantumcat-py/Snapshot-Report) | Timestamped "state of this machine" triage report |

Those three grew up into the toolkit above.

## Toolbox

Python · Linux · Wireshark · networking fundamentals · blue-team / SOC basics ·
learning in public, one broken script at a time
