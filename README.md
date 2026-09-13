# 1102tools

**Federal contracting prompts and MCP servers for working with official government sources.**

The prompts describe the job. The MCPs give your AI assistant tools to retrieve the source material. Use them together to research opportunities, awards, pricing, regulations, and policy changes.

[Browse the prompts](https://github.com/1102tools-dev/federal-contracting-prompts) · [Connect the MCPs](https://github.com/1102tools-dev/federal-contracting-mcps)

## Available in ChatGPT

Select MCPs are available in the ChatGPT directory. Install and connect them directly from these listings; no user API key or local setup is required.

- [USAspending](https://chatgpt.com/plugins/plugin_asdk_app_6a9ee668cc248191a0bdb9911b546799)
- [GSA CALC+](https://chatgpt.com/plugins/plugin_asdk_app_6a9eeeebfa8c81918945df0945276cb1)
- [eCFR](https://chatgpt.com/plugins/plugin_asdk_app_6a9ef0341b04819192935fd4e5cd9b34)

## Start with a question

1. Choose a request from the **prompts repository** and check its **Required MCPs** label.
2. Connect those servers using their individual setup instructions in the **MCP repository**. Configure any required API keys and confirm the tools are available in your client.
3. Replace placeholders such as `[AGENCY]`, `[COMPANY]`, or `[FAR PART]`, then send the request. Ask for source links, relevant dates, and any retrieval gaps.

A prompt does not install a server. If a required MCP is unavailable, connect it before relying on the answer as source-backed research.

## Match the work to the source

| What you want to do | MCP to connect | Matching prompts |
|---|---|---|
| Find solicitations and check company registrations | [SAM.gov](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/sam-gov-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#catching-opportunities) |
| Research awards, competitors, agencies, and recompetes | [USASpending](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/usaspending-gov-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#competitor-intelligence) |
| Compare awarded labor-rate ceilings | [GSA CALC+](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/gsa-calc-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#gsa-calc) |
| Look up occupation and location wage data | [BLS OEWS](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/bls-oews-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#bls-oews) |
| Estimate lodging and meals for travel | [GSA Per Diem](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/gsa-perdiem-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#gsa-per-diem) |
| Read and compare codified FAR, DFARS, and CFR text | [eCFR](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/ecfr-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#ecfr) |
| Follow proposed rules, final rules, and FAR cases | [Federal Register](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/federal-register-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#federal-register) |
| Explore rulemaking dockets and public comments | [Regulations.gov](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/regulations-gov-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#regulationsgov) |
| Research FAR Overhaul model text and posted agency deviations | [Acquisition.gov](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/acquisition-gov-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#far-overhaul-and-agency-deviations) |

## Combine sources when the question needs them

- **Competitor research:** USASpending shows award history; SAM.gov adds registration, exclusion, and opportunity records.
- **Labor pricing:** BLS supplies wage data; CALC+ supplies awarded ceiling rates; Per Diem adds travel rates. These are different inputs, not interchangeable prices.
- **Policy research:** eCFR provides codified text; Acquisition.gov provides FAR Overhaul model text and posted deviations; Federal Register and Regulations.gov provide rulemaking history and comments.

The prompt library includes requests for individual sources and combinations, with the required MCPs named beneath each request.

## Setup and availability

SAM.gov requires a user API key. BLS OEWS, GSA Per Diem, and Regulations.gov offer limited access without a user key. USASpending, GSA CALC+, eCFR, Federal Register, and Acquisition.gov require no user key. Follow each server's README for current configuration and access limits.

Browse the [prompt library](https://1102tools.com/#prompts), download the [September 2026 MCP Prompt Guide](https://1102tools.com/downloads/1102tools-prompt-guide.pdf), or use the repositories above for source code and installation instructions. The print guide covers the original eight sources; two additional Acquisition.gov examples are available online.

Built by James Jenrette. Free and open source. Independently developed and not affiliated with or endorsed by any federal agency. Research results support human judgment; they do not make contracting, legal, or procurement-specific applicability decisions.
