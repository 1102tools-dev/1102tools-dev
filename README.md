# 1102tools

Open federal acquisition AI agents for the government workforce and federal contracting industry.

Choose the job in front of you, install one agent package, and describe the work in ordinary language. The maintained setup paths are Codex Desktop and CLI, Claude Desktop (Code), and Claude Code CLI.

[Agents](https://github.com/1102tools-dev/federal-contracting-agents) · [Website](https://1102tools.com) · [Visible setup and API-key instructions](https://1102tools.com/setup) · [PDF guide](https://1102tools.com/downloads/1102tools-agent-setup-guide.pdf) · [How It Works](https://1102tools.com/examples)

## Five stable agents

| Agent | Work | Status |
|---|---|---|
| **Market Research Agent** | FAR Part 10 research, commerciality, competition, small-business availability, and market conditions | `1.0.1` stable |
| **Pre-Award Agent** | SOW/PWS development, IGCEs, and approved scope-to-pricing workflows | `1.0.1` stable |
| **GovCon Growth Agent** | Opportunities, competitors, recompetes, teaming, agencies, markets, and pricing context | `1.0.1` stable |
| **Other Transaction Agent** | Milestone-based OT project descriptions, cost analysis, revisions, and recosting | `1.0.1` stable |
| **Acquisition Policy Agent** | Codified rules, RFO status, deviations, rulemakings, comments, and policy impacts | `1.0.1` stable |

Market Research and GovCon Growth require approval before every public-web research run. Native web only is recommended; Tavily remains an explicitly selected optional provider and is never a silent fallback. Acquisition Policy reports documented status rather than legal advice or a procurement-specific applicability determination.

All five 1102tools agents are stable at `1.0.1`. They are installed from the GitHub-hosted 1102tools marketplace. The marketplace catalog itself is version [`1.2.1`](https://github.com/1102tools-dev/federal-contracting-agents/releases/tag/v1.2.1); that catalog version is separate from the agent package versions. Codex Desktop/CLI and Claude Code in Claude Desktop/CLI are the two maintained client families and four tested surfaces. Install or select the intended agent before giving the natural-language request; ambient routing remains host-controlled and best effort. This GitHub marketplace is the maintained distribution and is not an official platform storefront listing.

## Data access readiness

No 1102tools account is required; some federal providers require a free account or API key. Agent `1.0.1` checks credential presence locally before its workflow menu or routed response. The check never displays, transmits, logs, or validates the value.

| Agent | Credential state without user keys | What appears at startup |
|---|---|---|
| Market Research | `SAM_API_KEY` is required for SAM.gov operations | Missing required credential; only SAM-dependent work stops |
| GovCon Growth | `SAM_API_KEY` is required for SAM.gov operations | Missing required credential; never mislabels it as a SAM.gov outage |
| Pre-Award | `BLS_API_KEY` recommended; `PERDIEM_API_KEY` relevant to travel pricing | Limited BLS and Per Diem fallback warning; bounded work may continue |
| Other Transaction | `BLS_API_KEY` recommended; `PERDIEM_API_KEY` relevant to travel pricing | Limited BLS and Per Diem fallback warning; bounded work may continue |
| Acquisition Policy | `REGULATIONS_GOV_API_KEY` recommended | Limited Regulations.gov `DEMO_KEY` warning; bounded work may continue |

USASpending, GSA CALC+, eCFR, Federal Register, and Acquisition.gov need no user key. Get keys through [SAM.gov Help](https://sam.gov/help), [BLS registration](https://data.bls.gov/registrationEngine/), or [api.data.gov signup](https://api.data.gov/signup/). Configure credentials outside chat, fully restart the client, and rerun the workflow. Never paste a key into a conversation.

Agent `1.0.0` has a known missing-key diagnostic limitation: a failed keyed operation can be presented as a generic server failure. Update all five agents to `1.0.1` and, for multi-agent Codex installs, use the complete shared `1102tools-host` MCP configuration.

## Advanced building blocks

Most users should start with an agent. Developers and power users can inspect the components or maintain custom configurations:

- [Host-neutral workflow skills](https://github.com/1102tools-dev/federal-contracting-skills)
- [Federal source MCP servers](https://github.com/1102tools-dev/federal-contracting-mcps)
- [Advanced MCP-oriented request library](https://github.com/1102tools-dev/federal-contracting-prompts)

Built and maintained by a current lead systems analyst and contracting officer. 1102tools is independently developed and is not affiliated with or endorsed by any federal agency.

<!-- updated 2026-08-24 -->
