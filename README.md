# Konstantinos

Athens. I build tools around one question: **what did an AI agent actually do, and can you prove it?** Numbers come with their limits, mistakes included.

## Projects

### [OmniOS](https://github.com/ntinosgkiou-code/omnios) · agentdryrun Gateway
Make AI agents ask before they act, and keep a record nobody can quietly edit: per-customer rules, four-eyes approvals, a signed append-only log (RFC 9162 Merkle tree, Ed25519 checkpoints), independent witnesses that refuse a rewritten history, and evidence packs a third party verifies offline. FastAPI service, browser UI, Python SDK, CLI, Docker, 175 tests in CI.
*Portfolio project, development paused. Never used with a real customer; the known gaps are listed in [KNOWN-LIMITS](https://github.com/ntinosgkiou-code/omnios/blob/main/docs/KNOWN-LIMITS.md).*

### [agentdryrun](https://github.com/ntinosgkiou-code/agentdryrun) · open source, Apache-2.0
A dry run for AI coding agents: one command reads the Claude Code sessions on your machine and shows which commands your rules would have stopped (recursive deletes, force pushes, `curl | sh`, secret files read, uploads). Read-only, local, zero dependencies. Checked on 2,000 public agent runs: 14 of my first 49 alarms were my own bugs, and they are fixed ([how](https://github.com/ntinosgkiou-code/agentdryrun/blob/main/docs/VALIDATION-PUBLIC-RUNS.md)).

```bash
git clone https://github.com/ntinosgkiou-code/agentdryrun && cd agentdryrun && python -m agentdryrun scan
```

### [Ran-Tevu](https://github.com/ntinosgkiou-code/ran-tevu)
AI booking and back-office platform for Greek clinics: patients book through an AI chat, the clinic gets patient files, invoicing with Greek VAT rules, a consent-gated no-show recovery loop, Stripe billing, an AI voice receptionist and a FHIR R4 bridge. About 39,500 lines of Python, 64 test files.
*Portfolio project: it was offered to Greek clinics, did not reach paying customers, and has been offline since October 2026.*

### Other
- **[mcp-agent](https://github.com/ntinosgkiou-code/mcp-agent)**: an MCP server that gives Claude live football odds and team form, and flags matches where the market price and a naive form model disagree. A demonstration of MCP tool calling, not a betting signal.
- **[payout-to-pnl](https://github.com/ntinosgkiou-code/payout-to-pnl)**: a Claude plugin that turns Etsy, Shopify, PayPal and eBay payout exports into a monthly P&L, with all arithmetic in plain Python.

## How I work
The [build log](https://github.com/ntinosgkiou-code/agentdryrun/blob/main/BUILD-LOG.md) records what worked and what was wrong. Questions or bug reports: open an issue in the relevant repository.
