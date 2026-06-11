<h1 align="center">Yongshan Yu</h1>

<p align="center">
  <strong>Agent framework builder · AI-assisted engineering systems · Open-source automation</strong>
</p>

<p align="center">
  I build frameworks that make AI coding tools operate reliably inside real repositories.
</p>

<p align="center">
  <a href="https://github.com/yyswhsccc/druid-agentic-engineering-os">Druid</a> ·
  <a href="https://yyswhsccc.github.io/druid-agentic-engineering-os/">Portfolio</a> ·
  <a href="https://www.linkedin.com/in/yongshan-yu-195771319/">LinkedIn</a> ·
  <a href="mailto:yuyongshan573@gmail.com">Email</a>
</p>

---

<p align="center">
  <strong>Druid</strong><br>
  Agentic Engineering OS<br>
  Repo risk discovery → Patch + tests → PR review loop → Adaptive memory
</p>

<p align="center">
  <code>36-PR RustChain review queue</code> ·
  <code>47 merged PRs overall</code> ·
  <code>payout / bridge / UTXO / governance / security</code>
</p>

## Druid — an agent that ships

Druid is an autonomous engineering loop I designed and built. It turns a live
repository into an environment: risks, tests, CI, review feedback, maintainer
preferences, reward signals, and stop-loss decisions.

Its proving ground is [RustChain](https://github.com/Scottcjn/Rustchain), an open
blockchain with a live bounty economy. Druid is not a one-off AI prompt; it is a
low-touch framework for routine engineering work, with human-in-the-loop gates for
high-risk decisions, policy changes, and final approvals.

- scans live repositories for security, correctness, reliability, and bounty-shaped risks;
- writes bounded patches and regression tests;
- tracks CI/review outcomes and updates strategy from merge, rejection, reward, and risk signals.

```text
Scanner
  -> Risk & Value Classifier
  -> Decision Engine
  -> Patch / Test Generator
  -> PR + CI Tracker
  -> Adaptive Memory
  -> Strategy Update / Stop-loss
  -> back to Risk & Value Classifier

High-risk decisions -> Human-in-loop Gate -> Patch / Test Generator
```

## Public proof

Live GitHub audit on **2026-06-11**: **47 merged PRs overall**, including
**45 merged RustChain PRs**, plus a **36-PR open RustChain review queue**.
Open PRs below are review-queue evidence, not merged claims.

- **Money-path correctness:** [#6219](https://github.com/Scottcjn/Rustchain/pull/6219)
  merged signed-transfer nonce ordering with replay tests.
- **State integrity:** [#6188](https://github.com/Scottcjn/Rustchain/pull/6188)
  merged block-save atomicity around template production.
- **Security economics:** [#6667](https://github.com/Scottcjn/Rustchain/pull/6667)
  merged slasher evidence core; [#6838](https://github.com/Scottcjn/Rustchain/pull/6838)
  merged RPC rate limiting.
- **Payout exact-once:** [#7353](https://github.com/Scottcjn/Rustchain/pull/7353)
  opens repeated-withdrawal claim protection in the current review queue.
- **Bridge terminal integrity:** [#7343](https://github.com/Scottcjn/Rustchain/pull/7343)
  opens terminal-state race protection for bridge voids.
- **UTXO transaction atomicity:** [#7350](https://github.com/Scottcjn/Rustchain/pull/7350)
  opens pending nonce admission serialization.
- **Governance / bounty / browser boundaries:** [#7345](https://github.com/Scottcjn/Rustchain/pull/7345),
  [#7361](https://github.com/Scottcjn/Rustchain/pull/7361), and
  [#7379](https://github.com/Scottcjn/Rustchain/pull/7379) cover fee ordering,
  claimant state guards, and dashboard escaping.

Full RustChain evidence board → [docs/evidence.md](./docs/evidence.md)

## What this proves

| System capability | What Druid demonstrates |
|---|---|
| Agent framework design | A scanner, classifier, decision engine, patch/test generator, CI tracker, memory base, and stop-loss loop working as one system. |
| Security automation | Vulnerability-shaped discovery across payout, bridge, UTXO, governance, browser, and operational boundaries. |
| Developer productivity | Routine PR work becomes auditable, test-backed, review-aware, and low-touch after setup. |
| Transferability | Druid currently uses bounty and reward signals as one training environment, but the framework generalizes to any repository with issues, tests, CI, and review feedback. |

I do not just use AI coding tools. I build the operating loop that makes them
useful inside real engineering systems.

## Reinforcement learning direction

I'm studying reinforcement learning because Druid's next problem is exactly an
RL-shaped one: sparse rewards, delayed review feedback, shifting maintainer
preferences, reward hacking risk, and strategy updates under uncertainty.

- [Reinforcement Learning Study Notes](https://github.com/yyswhsccc/Reinforcement-Learning-Study-Notes)
- Current obsessions: continual learning, agents in environments that fight back

## Also built

**C.A.R.E.** — a gamified anti-harassment training project.

---

<p align="center"><em>
Off-screen: fantasy novel, self-made clothes, occasional rap. Druid handles the
bounties; I handle the plot.
</em></p>
