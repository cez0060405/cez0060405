### I run a personal AI agent like a production system

Long-term single-machine deployment of [Hermes Agent](https://github.com/NousResearch/hermes-agent) (by Nous Research) on Windows 11 — and the engineering that keeps it honest over months of daily use.

**📌 Featured: [personal-agent-ops](https://github.com/cez0060405/personal-agent-ops)** — battle-tested assets from that deployment:

- 🧪 **Decision-behavior regression suite** — 125 golden samples, 3 labels per sample; routing accuracy 91.2% → 97.6% measured across model swaps
- 🔍 **Provider dilution auditor** — catches silent model substitution behind subscription channels (anti-pollution questions + multi-sampling vs official API)
- 🛡️ **Stream watchdog** — unattended mid-stream-drop detection with auto-resume; append-only incident ledger, judged by data not vibes
- 🧩 **Skill-engineering samples** — aligned with the Agent Skills open standard

**🔧 Open source — NousResearch/hermes-agent**

- [#96764](https://github.com/NousResearch/hermes-agent/issues/96764) — scripting contract for `config set` (no `--quiet`, misleading confirmations in non-interactive runs)
- [#80946](https://github.com/NousResearch/hermes-agent/issues/80946) — Windows artifact paths opened as `C:\...` instead of `file://` URLs; my fix PR was closed after upstream re-architected the same area (issue still open, awaiting upstream's own fix)
- Version-anchored data points on config-write triage

> 个人级 Agent 工程：让 Agent 长期跑得对，比演示它能干什么更难。

<!-- metrics referenced above are reproducible from the linked repo's own results files -->
