# 1102tools

Open federal acquisition AI agents for the government workforce and federal contracting industry.

Choose the job in front of you, install one agent package, and describe the work in ordinary language. The maintained setup paths are Codex Desktop and CLI, Claude Desktop (Code), and Claude Code CLI.

[Agents](https://github.com/1102tools-dev/federal-contracting-agents) · [Website](https://1102tools.com) · [Agent Setup Guide](https://1102tools.com/downloads/1102tools-agent-setup-guide.pdf) · [How It Works](https://1102tools.com/examples)

## Five stable agents

| Agent | Work | Status |
|---|---|---|
| **Market Research Agent** | FAR Part 10 research, commerciality, competition, small-business availability, and market conditions | `1.0.0` stable |
| **Pre-Award Agent** | SOW/PWS development, IGCEs, and approved scope-to-pricing workflows | `1.0.0` stable |
| **GovCon Growth Agent** | Opportunities, competitors, recompetes, teaming, agencies, markets, and pricing context | `1.0.0` stable |
| **Other Transaction Agent** | Milestone-based OT project descriptions, cost analysis, revisions, and recosting | `1.0.0` stable |
| **Acquisition Policy Agent** | Codified rules, RFO status, deviations, rulemakings, comments, and policy impacts | `1.0.0` stable |

Market Research and GovCon Growth require approval before every public-web research run. Native web only is recommended; Tavily remains an explicitly selected optional provider and is never a silent fallback. Acquisition Policy reports documented status rather than legal advice or a procurement-specific applicability determination.

The stable marketplace release is [`v1.2.0`](https://github.com/1102tools-dev/federal-contracting-agents/releases/tag/v1.2.0). Codex Desktop/CLI and Claude Code in Claude Desktop/CLI are the two maintained client families and four tested surfaces. Install or select the intended agent before giving the natural-language request; ambient routing remains host-controlled and best effort. This GitHub marketplace is the maintained distribution and is not an official platform storefront listing.

## Advanced building blocks

Most users should start with an agent. Developers and power users can inspect the components or maintain custom configurations:

- [Host-neutral workflow skills](https://github.com/1102tools-dev/federal-contracting-skills)
- [Federal source MCP servers](https://github.com/1102tools-dev/federal-contracting-mcps)
- [Advanced MCP-oriented request library](https://github.com/1102tools-dev/federal-contracting-prompts)

Built and maintained by a current lead systems analyst and contracting officer. 1102tools is independently developed and is not affiliated with or endorsed by any federal agency.

<!-- updated 2026-08-23 -->
