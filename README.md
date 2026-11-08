# Konstantinos · On-chain strategy & risk validation

Athens · independent · fixed-scope engagements

Before you put capital into a strategy, a bot or a token, I find out whether it holds up against **real fees, latency and adversarial conditions**, and I hand you the evidence, not an opinion.
I don't sell trading signals or profit promises.

## What you can hire me for

| The problem | What you get | Timing |
|-------------|--------------|--------|
| *"Does this strategy actually make money after costs?"* | A **Strategy Reality Check**: a pre-registered backtest on real on-chain data (Base; Uniswap, Aerodrome) with LP fees, L2 gas and data fee, execution delay and stress tests, ending in a **GO / NO-GO** verdict, a written report and reproducible code | about 5 working days |
| *"Is this token safe to trade?"* | A **pre-trade safety check** for your bot or UI: honeypot and tax simulation, LP lock, ownership, proxy and holder-concentration checks. It refuses whenever it is in doubt | scoped per project |
| *"Why does my live result leak versus the backtest?"* | An **execution-friction diagnosis**: fee tiers, slippage, gas including the L2 data fee, latency modelling, and the exact assumptions that broke | scoped per project |
| *"I need a bot that does not blow up."* | A **Base/EVM bot** with fail-closed safety, a paper mode, tests and a fork test, delivered as code you own | scoped per project |

## Proof: [Base-QuantLab](https://github.com/ntinosgkiou-code/base-quantlab)

I built an on-chain quant lab and used it on myself: **14 pre-registered strategy configurations from six families were tested on real Base data, and none passed.**
Pass/fail gates were written before any result, ideas ran once on unseen windows, intervals were clustered by day, and the confidence level tightened as hypotheses piled up.

- **The outcome:** the answer was *no*, found in hours, with real data and no capital at risk. That is what a reality check is for.
- **Real-world modelling:** next-block fills on real pool reserves, the L2 data fee, and Base's move from 2 s to 0.2 s blocks located inside the data by bisection.
- **Safety infrastructure:** a fail-closed token validator, a state machine that freezes on latency spikes or reorgs, and a local mainnet-fork test with fake ETH (13 checks). 55 offline tests in CI.
- **Honest limits:** survivorship bias, approximations and what was *not* proven are stated in the repo.

## What I don't do

- I don't guarantee profit, give financial advice, or replace a smart-contract security audit.
- This is an early independent practice: I don't list past clients. Everything claimed here links to open code and data you can inspect.

## How I work

Rules are written before results. Failures are published with the numbers. The [build log](https://github.com/ntinosgkiou-code/agentdryrun/blob/main/BUILD-LOG.md) records what worked and what was wrong.

## Contact

Open an issue titled **`Reality check`** in [base-quantlab](https://github.com/ntinosgkiou-code/base-quantlab/issues), or in the repository closest to your question.

---

## More open work

### [OmniOS](https://github.com/ntinosgkiou-code/omnios) · agentdryrun Gateway
Make AI agents ask before they act, and keep a record nobody can quietly edit: per-customer rules, four-eyes approvals, a signed append-only log (RFC 9162 Merkle tree, Ed25519 checkpoints), independent witnesses that refuse a rewritten history, and evidence packs a third party verifies offline. FastAPI service, browser UI, Python SDK, CLI, Docker, 175 tests in CI.
*Portfolio project, development paused. Never used with a real customer; the known gaps are listed in [KNOWN-LIMITS](https://github.com/ntinosgkiou-code/omnios/blob/main/docs/KNOWN-LIMITS.md).*

### [agentdryrun](https://github.com/ntinosgkiou-code/agentdryrun) · open source, Apache-2.0
A dry run for AI coding agents: one command reads the Claude Code sessions on your machine and shows which commands your rules would have stopped (recursive deletes, force pushes, `curl | sh`, secret files read, uploads). Read-only, local, zero dependencies. Checked on 2,000 public agent runs: 14 of my first 49 alarms were my own bugs, and they are fixed ([how](https://github.com/ntinosgkiou-code/agentdryrun/blob/main/docs/VALIDATION-PUBLIC-RUNS.md)).

### [Ran-Tevu](https://github.com/ntinosgkiou-code/ran-tevu)
AI booking and back-office platform for Greek clinics: patients book through an AI chat, the clinic gets patient files, invoicing with Greek VAT rules, a consent-gated no-show recovery loop, Stripe billing, an AI voice receptionist and a FHIR R4 bridge. About 39,500 lines of Python, 64 test files.
*Portfolio project: it was offered to Greek clinics, did not reach paying customers, and has been offline since October 2026.*

### [token-tooling](https://github.com/ntinosgkiou-code/token-tooling)
Reference Solidity vesting and Merkle-airdrop contracts with fuzz and invariant tests (Foundry). Unaudited.
