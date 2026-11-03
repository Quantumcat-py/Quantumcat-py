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

## QuantumCat SOC Toolkit — v1.2 progress (November 2026)

- **Scanner:** Quick/Standard/Deep profiles (25/100/1000 ports), one retry on filtered ports, per-port latency, and expanded risky-port reasons.
- **Monitor + UI:** reverse-DNS peer names (labelled lookup results), live dark/light theme, and latency and retry display.
- **Analyst:** findings now carry latency, retry flags, subnet/gateway/DNS context, and peer names, with second-look rules for likely-firewall filtered counts and slow replies.
- **Honest status:** these are standalone script updates and app-side work in progress — the packaged app update is not live yet; it ships only when all three tools have something new to add.

Watch the v1.2 ad: https://www.youtube.com/shorts/jY6ccl56h80 — QuantumCat SOC Toolkit v1.2 is out — scanner profiles (25/100/1000 ports), retry + latency, peer hostnames, dark/light themes, and a smarter analyst. Still 100% local, still $12: https://quantumcatsoc.gumroad.com/l/quantumcat-soc-toolkit

## QuantumCat SOC Toolkit — v1.3 progress

- **Packet-level tracking (coming):** TCP and UDP packets, handshakes, flags, and flows — the toolkit currently watches connections, and v1.3 adds reading the packets themselves.
- **Analyst update:** it will fully read, understand, and analyze packet data, not just list endpoints.
- **Color-coded live packet feed:** built for people who like watching the feed live instead of only reading the analyst afterwards — categories are color-coded so things are easy to spot at a glance.
- **Fully customizable colors:** users can edit colors how they want, with a full color wheel and a large range of colors, plus presets.
- **Honest status:** v1.3 is in progress, not live yet; the packaged app on Gumroad is still v1.2.0 until v1.3 ships.
