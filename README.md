# Konstantinos · AI automation engineer

Athens · independent · fixed-scope work · NDA and white-label friendly

I build AI automations and agent workflows that are **tested, guarded and handed over with evidence**, so they keep working after the demo.
I work in two ways: as **delivery capacity for agencies and integrators** who sell AI solutions to their clients, and **directly with companies** that have one specific, costly manual process to automate.

## What I deliver

| You need | What you get |
|----------|--------------|
| **A delivery partner** (agency / integrator) | The AI automations and integrations you sold, built under your brand: agent workflows, voice and booking assistants, approval gates, billing and data integrations. Fixed scope, written acceptance criteria, tests, handover docs |
| **One costly process automated** (company) | A scoped project with a measurable acceptance test, human approval where actions are risky, and a record of what the automation did |
| **To know it works before it goes live** | A reality check on an automation, an agent or a strategy: pre-registered pass/fail criteria, real data, a written verdict and reproducible code |

## Selected work, grouped by what it proves

### Build: end-to-end AI products
**[Ran-Tevu](https://github.com/ntinosgkiou-code/ran-tevu)** · AI booking and back-office platform for clinics: patients book through an AI chat, invoicing with Greek VAT rules, a consent-gated no-show recovery loop, Stripe billing, an AI voice receptionist and a FHIR R4 bridge. About 39,500 lines of Python, 64 test files.
*Portfolio project, offline since October 2026; it did not reach paying customers.*

### Guard: control and evidence for AI agents
**[agentdryrun](https://github.com/ntinosgkiou-code/agentdryrun)** · open source, Apache-2.0. A dry run for coding agents: reads your Claude Code sessions and shows which commands your rules would have stopped. Checked on 2,000 public agent runs: 14 of my first 49 alarms were my own bugs, and they are fixed ([how](https://github.com/ntinosgkiou-code/agentdryrun/blob/main/docs/VALIDATION-PUBLIC-RUNS.md)).
**[OmniOS](https://github.com/ntinosgkiou-code/omnios)** · four-eyes approvals and a signed, append-only log for AI agents, with evidence packs a third party verifies offline. 175 tests in CI. *Portfolio project; known gaps in [KNOWN-LIMITS](https://github.com/ntinosgkiou-code/omnios/blob/main/docs/KNOWN-LIMITS.md).*

### Verify: test before you trust
**[Base-QuantLab](https://github.com/ntinosgkiou-code/base-quantlab)** · a lab that tested 14 pre-registered strategy configurations on real on-chain data; none passed, which was found in hours instead of after a launch. Pass/fail gates written before results, fail-closed safety checks, 55 tests, [decision records](https://github.com/ntinosgkiou-code/base-quantlab/blob/main/docs/DECISIONS.md).

### Also
**[voiceover-sync-skill](https://github.com/ntinosgkiou-code/voiceover-sync-skill)** · open source, MIT. A Claude Code skill that syncs a voiceover to a screen recording so every click lands on its spoken word, with burned-in captions, chapters and an automatic QA report. On a real onboarding video: 10 of 10 clicks within 0.4 s of their cue word, no freezes over 1.5 s. *Needs ffmpeg and faster-whisper; timeline anchors are still picked by the agent, not fully automatic.*
**[token-tooling](https://github.com/ntinosgkiou-code/token-tooling)** · reference Solidity vesting and Merkle-airdrop contracts with fuzz and invariant tests. Unaudited.

## How I work

- **Fixed scope and acceptance criteria in writing** before any build starts.
- **Small steps, tests, and a handover document** you can give to your own team or client.
- **Risky actions get a human approval gate** and every action leaves a record.
- **I say what I did not prove.** Every repo above lists its limits.

## Work with me

Email: **ntinosgkiou@gmail.com**
or open an issue titled **`Project`** in [Base-QuantLab](https://github.com/ntinosgkiou-code/base-quantlab/issues).
