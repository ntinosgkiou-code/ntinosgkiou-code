# Hi

I build small, useful open-source tools for people who run AI coding agents.

**Now: [agentdryrun](https://github.com/ntinosgkiou-code/agentdryrun)**, a dry run on your own coding agent's history. One command reads the Claude Code sessions on your machine and shows which commands your rules would have stopped: recursive deletes, force pushes, `curl | sh`, secret files read, uploads. Read-only, local, zero dependencies.

```bash
git clone https://github.com/ntinosgkiou-code/agentdryrun && cd agentdryrun && python -m agentdryrun scan
```

Or inside Claude Code: `claude plugin marketplace add ntinosgkiou-code/agentdryrun`, then `claude plugin install agentdryrun@agentdryrun` and `/agentdryrun:scan`.

It is a prototype and the [build log](https://github.com/ntinosgkiou-code/agentdryrun/blob/main/BUILD-LOG.md) records what worked and what was wrong. If you try it on your own history, the most useful thing you can send is where it is wrong: [open an issue](https://github.com/ntinosgkiou-code/agentdryrun/issues).
