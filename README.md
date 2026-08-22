# 1102tools

Free, open tooling for federal contracting, built for GS-1102s and small businesses.

Built and maintained by a current lead systems analyst and contracting officer. 1102tools is independently developed and is not affiliated with or endorsed by any federal agency.

[Skills](https://github.com/1102tools-dev/federal-contracting-skills) · [MCPs](https://github.com/1102tools-dev/federal-contracting-mcps) · [Agents](https://github.com/1102tools-dev/federal-contracting-agents) · [Prompts](https://github.com/1102tools-dev/federal-contracting-prompts) · [Site](https://1102tools.com)

## Roadmap

**Prompts: shipped.** The prompt guide is now a repo: [federal-contracting-prompts](https://github.com/1102tools-dev/federal-contracting-prompts), 60 field-tested prompts as browsable, copy-paste markdown. The repo is the canonical home of the library; the PDF is rebuilt from it.

**MCPs: safety release shipped.** All eight servers now include provisional anti-burst pacing with cross-process coordination on one computer, explicit override controls, and conservative 3- or 4-second defaults. The individually versioned PyPI packages were published together from monorepo release `v1.0.9` after 3,464 offline tests. The safeguard reduces accidental bursts but is not a provider guarantee or daily-quota manager.

**Skills: refreshed.** All six skills were modernized on August 21, 2026 as portable, progressive-disclosure packages rather than monolithic Markdown prompts. Each now includes a compact orchestration core, supporting references, deterministic workbook or document validators, and a current `test.md`. OpenAI Codex using GPT-5.6 Sol completed the restructure and testing pass. Behavioral gates were exercised in Codex CLI with GPT-5.6 Sol at xhigh reasoning and Claude Code CLI with Opus 5; FFP also received claude.ai Opus 5 Max and Codex Desktop coverage. The refreshed skills are live in [federal-contracting-skills](https://github.com/1102tools-dev/federal-contracting-skills).

**Agents: public preview.** The Pre-Award Agent and Other Transaction Agent are available at `1.0.0-rc.3` through repository marketplaces for Codex, Claude Code, and Copilot CLI. Each self-contained Agent Plugins 1.0 package combines a portable orchestrator, the complete multi-file skills for its workflow, and the three pinned pricing MCP definitions it needs. The `rc.3` release adopts the new MCP pacing safeguards without changing acquisition logic. Final `1.0.0` remains gated on the documented authenticated-client and end-to-end artifact matrix. See [federal-contracting-agents](https://github.com/1102tools-dev/federal-contracting-agents) and the [Universal Setup Guide](https://1102tools.com/downloads/1102tools-universal-setup.pdf).

<!-- updated 2026-08-21 -->
