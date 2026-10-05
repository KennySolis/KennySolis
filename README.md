# Kenny Solis

Underwriting professional who designs, builds, and operates production automation
end-to-end — computer vision, API integration, and the unglamorous ops work that
keeps systems alive.

**Running in production:**

- **[card-pipeline](https://github.com/KennySolis/card-pipeline)** — computer-vision
  pipeline taking physical trading cards from camera scan to live eBay listing.
  Hosted vision LLMs (Google Gemini, multi-provider), 20k-card reference database,
  full eBay Trading/Sell/OAuth integration, self-healing service watchdog, Linux VPS
  deploy. In production since February 2026.
- **[fleet](https://github.com/KennySolis/fleet)** — capability-based job
  dispatcher across a heterogeneous personal compute fleet (7 nodes, 3
  machines): health probing, measured cost ranking, GPU mutex groups that
  serialize LLM inference vs image generation, Wake-on-LAN power control,
  JSONL job journal + live dashboard.

**Also built:**

- **[audit-guide](https://github.com/KennySolis/audit-guide)** — local-first
  computer-vision workflow guide: a FastAPI app that walks a physical audit or
  verification task step by step with a locally hosted vision model in the loop.
  Raw camera frames stay in memory and are never written to disk; runs entirely
  on the local network.

**Day job:** Underwriting Service Assistant (S3) at a major insurer — daily
underwriting-audit review in mainframe-based policy systems, plus Excel VBA
automation attached to live terminal-emulation sessions.

**Tools:** Python (Flask, FastAPI) · VBA · PowerShell · SQL · REST APIs ·
systemd/nginx/TLS · Git

fleet is the real dispatcher code, lightly sanitized. card-pipeline and
audit-guide are sanitized overviews of private working systems (card-pipeline
includes its real production watchdog). Implementation walkthrough available
on request.
