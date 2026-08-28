# 1102tools

Open federal acquisition AI agents for the government workforce and federal contracting industry.

Choose the job in front of you, install one agent package, and describe the work in ordinary language. The maintained setup paths are Codex Desktop and CLI, Claude Desktop (Code), and Claude Code CLI.

[Agents](https://github.com/1102tools-dev/federal-contracting-agents) · [Complete menu-to-outcome map](https://1102tools.com/tools#outcome-map-title) · [Optional Agent Playbook](https://github.com/1102tools-dev/federal-contracting-prompts#recommended-agent-playbook) · [Visible setup and API-key instructions](https://1102tools.com/setup) · [PDF guide](https://1102tools.com/downloads/1102tools-agent-setup-guide.pdf) · [How It Works](https://1102tools.com/examples)

## No special prompt is required to start

You do not need to memorize commands or write a long prompt.

- **Codex Desktop or CLI:** type `@`, begin typing the agent name, and wait for the matching agent to appear.
- **Claude Code in Desktop or CLI:** type `/`, begin typing the agent name, and wait for its workflow to appear.
- In either client, press Enter once to load the autocomplete into the prompt box, then press Enter again to send it and start the agent. After the first Enter, you may add an ordinary-language request before sending.
- Choose the closest numbered route. If you are unsure, select **Help me choose**.
- The agent will name the recommended deliverable, explain what it includes, identify the decisions that remain yours, and ask for the next specific fact or approval it needs.

The user should not have to invent a report or know the product catalog in advance. The complete route map names all 33 default outcomes. The optional Agent Playbook adds ambitious examples for users who want to see the full reach of a route; it does not bypass readiness, source-plan, artifact, pricing-method, or CO/AO authority gates.

## Five stable agents

| Agent | Work | Status |
|---|---|---|
| **GovCon Growth Agent** | Opportunities, competitors, recompetes, teaming, agencies, markets, and pricing context | `1.0.3` stable |
| **Market Research Agent** | FAR Part 10 research, commerciality, competition, small-business availability, and market conditions | `1.0.3` stable |
| **Pre-Award Agent** | SOW/PWS development, IGCEs, and approved scope-to-pricing workflows | `1.0.3` stable |
| **Other Transaction Agent** | Milestone-based OT project descriptions, cost analysis, revisions, and recosting | `1.0.3` stable |
| **Acquisition Policy Agent** | Codified rules, RFO status, deviations, rulemakings, comments, and policy impacts | `1.0.3` stable |

Market Research and GovCon Growth require approval before every public-web research run. Native web only is recommended; Tavily remains an explicitly selected optional provider and is never a silent fallback. Acquisition Policy reports documented status rather than legal advice or a procurement-specific applicability determination.

All five 1102tools agents are stable at `1.0.3`. They are installed from the GitHub-hosted 1102tools marketplace. The marketplace catalog itself is version [`1.2.3`](https://github.com/1102tools-dev/federal-contracting-agents/releases/tag/v1.2.3); that catalog version is separate from the agent package versions. Codex Desktop/CLI and Claude Code in Claude Desktop/CLI are the two maintained client families and four tested surfaces. Install or select the intended agent before giving the natural-language request; ambient routing remains host-controlled and best effort. This GitHub marketplace is the maintained distribution and is not an official platform storefront listing.

## Data access readiness

No 1102tools account is required; some federal providers require a free account or API key. Agent `1.0.3` checks credential presence locally before its workflow menu or routed response. The check never displays, transmits, logs, or validates the value.

| Agent | Credential state without user keys | What appears at startup |
|---|---|---|
| GovCon Growth | `SAM_API_KEY` is required for SAM.gov operations | Missing required credential; never mislabels it as a SAM.gov outage |
| Market Research | `SAM_API_KEY` is required for SAM.gov operations | Missing required credential; only SAM-dependent work stops |
| Pre-Award | `BLS_API_KEY` recommended; `PERDIEM_API_KEY` relevant to travel pricing | Limited BLS and Per Diem fallback warning; bounded work may continue |
| Other Transaction | `BLS_API_KEY` recommended; `PERDIEM_API_KEY` relevant to travel pricing | Limited BLS and Per Diem fallback warning; bounded work may continue |
| Acquisition Policy | `REGULATIONS_GOV_API_KEY` recommended | Limited Regulations.gov `DEMO_KEY` warning; bounded work may continue |

USASpending, GSA CALC+, eCFR, Federal Register, and Acquisition.gov need no user key. Get keys through [SAM.gov Help](https://sam.gov/help), [BLS registration](https://data.bls.gov/registrationEngine/), or [api.data.gov signup](https://api.data.gov/signup/). Configure credentials outside chat, fully restart the client, and rerun the workflow. Never paste a key into a conversation.

Agent `1.0.0` has a known missing-key diagnostic limitation: a failed keyed operation can be presented as a generic server failure. Update all five agents to `1.0.3` and, for multi-agent Codex installs, use the complete shared `1102tools-host` MCP configuration.

## Advanced building blocks

Most users should start with an agent. Developers and power users can inspect the components or maintain custom configurations:

- [Host-neutral workflow skills](https://github.com/1102tools-dev/federal-contracting-skills)
- [Federal source MCP servers](https://github.com/1102tools-dev/federal-contracting-mcps)
- [Optional Agent Playbook and advanced Direct-MCP Library](https://github.com/1102tools-dev/federal-contracting-prompts)

Built and maintained by a current lead systems analyst and contracting officer. 1102tools is independently developed and is not affiliated with or endorsed by any federal agency.

<!-- updated 2026-08-28 -->
