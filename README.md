# 1102tools

Free, open tooling for federal contracting, built for GS-1102s and small businesses.

Built and maintained by a current lead systems analyst and contracting officer. 1102tools is independently developed and is not affiliated with or endorsed by any federal agency.

[Skills](https://github.com/1102tools-dev/federal-contracting-skills) · [MCPs](https://github.com/1102tools-dev/federal-contracting-mcps) · [Agents](https://github.com/1102tools-dev/federal-contracting-agents) · [Prompts](https://github.com/1102tools-dev/federal-contracting-prompts) · [Site](https://1102tools.com)

## Roadmap

**Prompts: shipped.** The prompt guide is now a repo: [federal-contracting-prompts](https://github.com/1102tools-dev/federal-contracting-prompts), 62 copy-paste prompts as browsable Markdown. Sixty MCP patterns were field-tested against live sources; two no-call launch prompts open the new research-agent menus. The repo is the canonical home of the library; the PDF is rebuilt from it.

**MCPs: safety release shipped.** All eight servers now include provisional anti-burst pacing with cross-process coordination on one computer, explicit override controls, and conservative 3- or 4-second defaults. The individually versioned PyPI packages were published together from monorepo release `v1.0.9` after 3,464 offline tests. The safeguard reduces accidental bursts but is not a provider guarantee or daily-quota manager.

**Skills: eight complete packages.** The six document and pricing skills were modernized on August 21, 2026 as portable, progressive-disclosure packages rather than monolithic prompts. Market Research Builder and GovCon Growth Workflow add document-aware acquisition research and industry growth intelligence, each with a mandatory launch menu, per-run web-provider approval, traceable evidence record, deterministic artifact validators, and a current `test.md`. The skills support host-native search, optional Tavily, or no public web; Tavily is never the sole path and receives only approved sanitized public terms or URLs. Behavioral gates were exercised in Codex CLI with GPT-5.6 Sol at xhigh reasoning and Claude Code CLI with resolved Opus 5 at max effort; a Sonnet question-omission regression was fixed and passed on fresh runs. The canonical packages are live in [federal-contracting-skills](https://github.com/1102tools-dev/federal-contracting-skills).

**Agents: four public previews.** Pre-Award Agent and Other Transaction Agent remain at `1.0.0-rc.3`. GovCon Growth Agent and Market Research Agent are at `1.0.0-rc.2` in repository release `v1.1.0-rc.2`. The two research agents configure Tavily's official keyless remote MCP as an optional third-party capability alongside native host search. Every research run requires explicit provider and sanitized-query approval; users may select native only or no public web, and complete opt-out is documented. Clean marketplace installation and inventory passed in Codex CLI, Claude Code, and Copilot CLI. Tavily initialization/tool discovery and a limited live search check passed without any federal API call. Final `1.0.0` remains gated on the documented client, live-source, routing, and artifact matrix. See [federal-contracting-agents](https://github.com/1102tools-dev/federal-contracting-agents) and the [Universal Setup Guide](https://1102tools.com/downloads/1102tools-universal-setup.pdf).

<!-- updated 2026-08-21 -->
