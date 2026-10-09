# 1102tools

[![GitHub stars](https://img.shields.io/github/stars/1102tools-dev/federal-contracting-mcps?style=flat&color=e3b341&logo=github&logoColor=white&label=stars)](https://github.com/1102tools-dev/federal-contracting-mcps/stargazers) [![PyPI downloads: 100k+](https://img.shields.io/badge/PyPI%20downloads-100k%2B-1f6feb?logo=pypi&logoColor=white)](https://github.com/1102tools-dev/federal-contracting-mcps#server-catalog) [![PyPI: 9 packages](https://img.shields.io/badge/PyPI-9%20packages-1f6feb?logo=pypi&logoColor=white)](https://github.com/1102tools-dev/federal-contracting-mcps#server-catalog)

[![price: free](https://img.shields.io/badge/price-free-007a59)](https://1102tools.com/#why) [![license: MIT](https://img.shields.io/badge/license-MIT-007a59)](https://github.com/1102tools-dev/federal-contracting-mcps/blob/main/license) [![tools: 133](https://img.shields.io/badge/tools-133-007a59)](https://github.com/1102tools-dev/federal-contracting-mcps) [![regression tests: 5,571](https://img.shields.io/badge/regression%20tests-5%2C571-007a59)](https://github.com/1102tools-dev/federal-contracting-mcps#testing-and-maintenance) [![prompts: 56](https://img.shields.io/badge/prompts-56-007a59)](https://github.com/1102tools-dev/federal-contracting-prompts)

[![Claude directory: 9 servers](https://img.shields.io/badge/Claude%20directory-9%20servers-6f42c1?logo=claude&logoColor=white)](#local-or-hosted) [![ChatGPT directory: 4 servers](https://img.shields.io/badge/ChatGPT%20directory-4%20servers-6f42c1?logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyBmaWxsPSJ3aGl0ZSIgcm9sZT0iaW1nIiB2aWV3Qm94PSIwIDAgMjQgMjQiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI%2BPHRpdGxlPk9wZW5BSTwvdGl0bGU%2BPHBhdGggZD0iTTIyLjI4MTkgOS44MjExYTUuOTg0NyA1Ljk4NDcgMCAwIDAtLjUxNTctNC45MTA4IDYuMDQ2MiA2LjA0NjIgMCAwIDAtNi41MDk4LTIuOUE2LjA2NTEgNi4wNjUxIDAgMCAwIDQuOTgwNyA0LjE4MThhNS45ODQ3IDUuOTg0NyAwIDAgMC0zLjk5NzcgMi45IDYuMDQ2MiA2LjA0NjIgMCAwIDAgLjc0MjcgNy4wOTY2IDUuOTggNS45OCAwIDAgMCAuNTExIDQuOTEwNyA2LjA1MSA2LjA1MSAwIDAgMCA2LjUxNDYgMi45MDAxQTUuOTg0NyA1Ljk4NDcgMCAwIDAgMTMuMjU5OSAyNGE2LjA1NTcgNi4wNTU3IDAgMCAwIDUuNzcxOC00LjIwNTggNS45ODk0IDUuOTg5NCAwIDAgMCAzLjk5NzctMi45MDAxIDYuMDU1NyA2LjA1NTcgMCAwIDAtLjc0NzUtNy4wNzI5em0tOS4wMjIgMTIuNjA4MWE0LjQ3NTUgNC40NzU1IDAgMCAxLTIuODc2NC0xLjA0MDhsLjE0MTktLjA4MDQgNC43NzgzLTIuNzU4MmEuNzk0OC43OTQ4IDAgMCAwIC4zOTI3LS42ODEzdi02LjczNjlsMi4wMiAxLjE2ODZhLjA3MS4wNzEgMCAwIDEgLjAzOC4wNTJ2NS41ODI2YTQuNTA0IDQuNTA0IDAgMCAxLTQuNDk0NSA0LjQ5NDR6bS05LjY2MDctNC4xMjU0YTQuNDcwOCA0LjQ3MDggMCAwIDEtLjUzNDYtMy4wMTM3bC4xNDIuMDg1MiA0Ljc4MyAyLjc1ODJhLjc3MTIuNzcxMiAwIDAgMCAuNzgwNiAwbDUuODQyOC0zLjM2ODV2Mi4zMzI0YS4wODA0LjA4MDQgMCAwIDEtLjAzMzIuMDYxNUw5Ljc0IDE5Ljk1MDJhNC40OTkyIDQuNDk5MiAwIDAgMS02LjE0MDgtMS42NDY0ek0yLjM0MDggNy44OTU2YTQuNDg1IDQuNDg1IDAgMCAxIDIuMzY1NS0xLjk3MjhWMTEuNmEuNzY2NC43NjY0IDAgMCAwIC4zODc5LjY3NjVsNS44MTQ0IDMuMzU0My0yLjAyMDEgMS4xNjg1YS4wNzU3LjA3NTcgMCAwIDEtLjA3MSAwbC00LjgzMDMtMi43ODY1QTQuNTA0IDQuNTA0IDAgMCAxIDIuMzQwOCA3Ljg3MnptMTYuNTk2MyAzLjg1NThMMTMuMTAzOCA4LjM2NCAxNS4xMTkyIDcuMmEuMDc1Ny4wNzU3IDAgMCAxIC4wNzEgMGw0LjgzMDMgMi43OTEzYTQuNDk0NCA0LjQ5NDQgMCAwIDEtLjY3NjUgOC4xMDQydi01LjY3NzJhLjc5Ljc5IDAgMCAwLS40MDctLjY2N3ptMi4wMTA3LTMuMDIzMWwtLjE0Mi0uMDg1Mi00Ljc3MzUtMi43ODE4YS43NzU5Ljc3NTkgMCAwIDAtLjc4NTQgMEw5LjQwOSA5LjIyOTdWNi44OTc0YS4wNjYyLjA2NjIgMCAwIDEgLjAyODQtLjA2MTVsNC44MzAzLTIuNzg2NmE0LjQ5OTIgNC40OTkyIDAgMCAxIDYuNjgwMiA0LjY2ek04LjMwNjUgMTIuODYzbC0yLjAyLTEuMTYzOGEuMDgwNC4wODA0IDAgMCAxLS4wMzgtLjA1NjdWNi4wNzQyYTQuNDk5MiA0LjQ5OTIgMCAwIDEgNy4zNzU3LTMuNDUzN2wtLjE0Mi4wODA1TDguNzA0IDUuNDU5YS43OTQ4Ljc5NDggMCAwIDAtLjM5MjcuNjgxM3ptMS4wOTc2LTIuMzY1NGwyLjYwMi0xLjQ5OTggMi42MDY5IDEuNDk5OHYyLjk5OTRsLTIuNTk3NCAxLjQ5OTctMi42MDY3LTEuNDk5N1oiLz48L3N2Zz4%3D)](#local-or-hosted) [![Cloudflare Workers](https://img.shields.io/badge/hosted%20on-Cloudflare%20Workers-F38020?logo=cloudflare&logoColor=white)](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/deploy)

**Free, open-source federal contracting prompts and MCP servers for working with official government sources.**

The prompts describe the job. The MCPs give your AI assistant tools to retrieve the source material. Use them together to research opportunities, awards, pricing, regulations, and policy changes.

[Browse the prompts](https://github.com/1102tools-dev/federal-contracting-prompts) · [Connect the MCPs](https://github.com/1102tools-dev/federal-contracting-mcps)

## Why 1102tools

- **Free.** MIT-licensed, with no subscription and no credits. Directory installs need no account or API key.
- **Tested.** 5,571 collected regression tests, including live-API tests, across 9 servers and 133 tools, with up to ten audit rounds per server against the live government APIs. Published testing records document each bug fixed and the tests added.
- **Listed, no keys.** All 9 servers are in the Claude directory and 4 are in the ChatGPT directory, with the rest in review for ChatGPT. Directory installs need no user API key.
- **One of a kind.** The only known MCP server for Acquisition.gov FAR Overhaul model text and agency class deviations.

See [how 1102tools compares](https://1102tools.com/compare) with paid GovCon platforms and other MCP servers.

<a id="available-in-claude-and-chatgpt"></a>

## Local or hosted

Every MCP works in Claude or ChatGPT two ways. **Local** runs it on your computer, inside the Claude or ChatGPT desktop app or another AI app. **Hosted** runs it on Cloudflare, so it works anywhere you use Claude or ChatGPT. Local is the better setup for daily work, and you don't have to set it up by hand: give your AI the [local setup guide](https://github.com/1102tools-dev/federal-contracting-mcps#local-setup) and ask it to set it up or walk you through it.

All nine are in the Claude directory and four are in ChatGPT as hosted installs. The rest are in review for ChatGPT.

| MCP | Local setup (desktop) | Claude (hosted) | ChatGPT (hosted) |
|---|---|---|---|
| SAM.gov | [Setup guide](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/sam-gov-mcp#installation) (full 20-tool edition, free key) | [Add to Claude](https://claude.ai/directory/sam-gov-by-1102tools) (4-tool edition, no key) | In review |
| USAspending | [Setup guide](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/usaspending-gov-mcp#installation) | [Add to Claude](https://claude.ai/directory/usaspending-by-1102tools) | [Add to ChatGPT](https://chatgpt.com/plugins/plugin_asdk_app_6a9ee668cc248191a0bdb9911b546799) |
| GSA CALC+ | [Setup guide](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/gsa-calc-mcp#installation) | [Add to Claude](https://claude.ai/directory/gsa-calc-by-1102tools) | [Add to ChatGPT](https://chatgpt.com/plugins/plugin_asdk_app_6a9eeeebfa8c81918945df0945276cb1) |
| BLS OEWS | [Setup guide](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/bls-oews-mcp#installation) | [Add to Claude](https://claude.ai/directory/bls-oews-by-1102tools) | In review |
| GSA Per Diem | [Setup guide](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/gsa-perdiem-mcp#installation) (free key) | [Add to Claude](https://claude.ai/directory/gsa-perdiem-by-1102tools) | In review |
| eCFR | [Setup guide](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/ecfr-mcp#installation) | [Add to Claude](https://claude.ai/directory/ecfr-by-1102tools) | [Add to ChatGPT](https://chatgpt.com/plugins/plugin_asdk_app_6a9ef0341b04819192935fd4e5cd9b34) |
| Acquisition.gov | [Setup guide](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/acquisition-gov-mcp#install) | [Add to Claude](https://claude.ai/directory/acquisition-gov-by-1102tools) | [Add to ChatGPT](https://chatgpt.com/plugins/plugin_asdk_app_6ab2757102e08191887f75cc506c2333) |
| Federal Register | [Setup guide](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/federal-register-mcp#installation) | [Add to Claude](https://claude.ai/directory/federal-register-by-1102tools) | In review |
| Regulations.gov | [Setup guide](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/regulations-gov-mcp#installation) (free key) | [Add to Claude](https://claude.ai/directory/regulations-gov-by-1102tools) | In review |

| | Local | Hosted |
|---|---|---|
| **Works in** | Claude or ChatGPT desktop apps, and other AI apps | Claude or ChatGPT on web, desktop, and phone |
| **Setup** | Ask your AI to set it up or walk you through it, using the setup guide. Free keys for 3 servers | One click. No keys |
| **Rate limits** | Your own | Pooled across all users. Your lookups stay private |
| **Relies on** | Your computer | Cloudflare and 1102tools being up |
| **SAM.gov** | Full edition: 20 tools, free key | 4 tools, no key |

**Use hosted if** you're on your phone, your work computer blocks installs, or you want SAM.gov opportunity search without a key.

- **SAM.gov comes in two editions.** The directory version (in the Claude directory) has 4 keyless tools for contract opportunities, award notices, and justifications. The full version has 20 tools and adds entity registrations, SBA certifications, exclusions, and contract award records. It needs a free SAM.gov key and a local install; there is no one-click directory install for it. [Compare the editions](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/sam-gov-mcp#two-editions-hosted-or-full).
- **Hosted privacy.** The hosted servers don't store your queries, results, or conversations, and request logging is turned off. Their code and Cloudflare setup are public in [federal-contracting-mcps](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/deploy). Cloudflare still handles connection data such as IP addresses, and Claude or ChatGPT handles your conversation under its own privacy policy.

[Local setup guide](https://github.com/1102tools-dev/federal-contracting-mcps#local-setup). You don't have to do it by hand: give your AI the link and ask it to set it up.

## Start with a question

1. Choose a request from the **prompts repository** and check its **Required MCPs** label.
2. Connect those servers: set them up locally from their setup guides in the **MCP repository**, or install the hosted versions from the Claude and ChatGPT directories. Configure any required API keys and confirm the tools are available in your client.
3. Replace placeholders such as `[AGENCY]`, `[COMPANY]`, or `[FAR PART]`, then send the request. Ask for source links, relevant dates, and any retrieval gaps.

A prompt does not install a server. If a required MCP is unavailable, connect it before relying on the answer as source-backed research.

## Match the work to the source

| What you want to do | MCP to connect | Matching prompts |
|---|---|---|
| Find solicitations and check company registrations | [SAM.gov](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/sam-gov-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#catching-opportunities) |
| Research awards, competitors, agencies, and recompetes | [USAspending](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/usaspending-gov-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#competitor-intelligence) |
| Compare awarded labor-rate ceilings | [GSA CALC+](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/gsa-calc-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#gsa-calc) |
| Look up occupation and location wage data | [BLS OEWS](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/bls-oews-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#bls-oews) |
| Estimate lodging and meals for travel | [GSA Per Diem](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/gsa-perdiem-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#gsa-per-diem) |
| Read and compare codified FAR, DFARS, and CFR text | [eCFR](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/ecfr-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#ecfr) |
| Research FAR Overhaul model text and posted agency deviations | [Acquisition.gov](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/acquisition-gov-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#far-overhaul-and-agency-deviations) |
| Follow proposed rules, final rules, and FAR cases | [Federal Register](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/federal-register-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#federal-register) |
| Explore rulemaking dockets and public comments | [Regulations.gov](https://github.com/1102tools-dev/federal-contracting-mcps/tree/main/servers/regulations-gov-mcp) | [Open prompts](https://github.com/1102tools-dev/federal-contracting-prompts#regulationsgov) |

## Combine sources when the question needs them

- **Competitor research:** USAspending shows award history; SAM.gov adds opportunity records, plus registration and exclusion records from its full local edition.
- **Labor pricing:** BLS supplies wage data; CALC+ supplies awarded ceiling rates; Per Diem adds travel rates. These are different inputs, not interchangeable prices.
- **Policy research:** eCFR provides codified text; Acquisition.gov provides FAR Overhaul model text and posted deviations; Federal Register and Regulations.gov provide rulemaking history and comments.

The prompt library includes requests for individual sources and combinations, with the required MCPs named beneath each request.

## Setup and availability

The full local SAM.gov server (20 tools) requires a free user API key; a keyless hosted edition with 4 tools for contract opportunities is in the Claude directory, with ChatGPT in review. GSA Per Diem and Regulations.gov need a free user key locally (Per Diem's ZIP, state, and M&IE lookups work without one); their hosted editions need no user key and are in the Claude directory, with ChatGPT in review. USAspending, GSA CALC+, BLS OEWS, eCFR, Federal Register, and Acquisition.gov require no user key, locally or hosted. Follow each server's README for current configuration and access limits.

Browse the [prompt library](https://1102tools.com/#prompts), download the [September 2026 MCP Prompt Guide](https://1102tools.com/downloads/1102tools-prompt-guide.pdf), or use the repositories above for source code and installation instructions. The print guide covers all 56 prompts across the nine sources.

Built by James Jenrette. Free and open source. Independently developed and not affiliated with or endorsed by any federal agency. Research results support human judgment; they do not make contracting, legal, or procurement-specific applicability decisions.
