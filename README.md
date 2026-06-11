# Yongshan Yu

I build **agentic engineering systems** that make AI coding tools operate reliably inside real repositories.

My flagship project is **Druid**, an agentic engineering operating system for PR work: issue discovery, vulnerability/risk-surface scanning, duplicate checks, scoped patch generation, tests, CI/review tracking, adaptive memory, and stop-loss.

**I do not just use AI tools. I build the framework that makes AI tools operate reliably.**

The hiring signal is not that I can manually operate one bot. It is that I can build low-touch internal agent frameworks for a company's own repositories, issue systems, review process, CI, docs, risk rules, and business goals.

## This Week Dashboard

Last audited: **2026-06-11**.

**Druid generated a 36-PR test-backed review queue across payout exact-once semantics, bridge terminal-state integrity, UTXO transaction atomicity, governance accounting, bounty attribution, browser/security boundaries, and operational reliability hardening.**

This is not a raw-count flex. The value is that Druid systematically scanned a complex codebase for vulnerability-shaped risks and reliability failures, cut them into small reviewable PRs, added tests and risk-boundary notes, and kept tracking CI/review/merge state.

| Surface | Example PRs | What Druid Found |
|---|---|---|
| Payout exact-once semantics | [#7385](https://github.com/Scottcjn/Rustchain/pull/7385), [#7357](https://github.com/Scottcjn/Rustchain/pull/7357), [#7353](https://github.com/Scottcjn/Rustchain/pull/7353) | Missing-row, terminal-status, and repeated-claim failure modes in payout paths. |
| Bridge terminal-state integrity | [#7363](https://github.com/Scottcjn/Rustchain/pull/7363), [#7343](https://github.com/Scottcjn/Rustchain/pull/7343), [#7316](https://github.com/Scottcjn/Rustchain/pull/7316) | Bridge state visibility, terminal race protection, and operator-only flow clarity. |
| UTXO transaction atomicity | [#7350](https://github.com/Scottcjn/Rustchain/pull/7350), [#7339](https://github.com/Scottcjn/Rustchain/pull/7339), [#7335](https://github.com/Scottcjn/Rustchain/pull/7335), [#7333](https://github.com/Scottcjn/Rustchain/pull/7333) | Nonce serialization, transaction ownership, conservation checks, and rollback edges. |
| Governance accounting | [#7347](https://github.com/Scottcjn/Rustchain/pull/7347), [#7345](https://github.com/Scottcjn/Rustchain/pull/7345) | Pagination and proposal-fee accounting paths that could create silent drift or unfair charging. |
| Bounty attribution / claims | [#7367](https://github.com/Scottcjn/Rustchain/pull/7367), [#7361](https://github.com/Scottcjn/Rustchain/pull/7361), [#7359](https://github.com/Scottcjn/Rustchain/pull/7359), [#7383](https://github.com/Scottcjn/Rustchain/pull/7383) | Claim completion, persistence, missing status rows, and honest reward/receipt messaging. |
| Browser/security boundaries | [#7382](https://github.com/Scottcjn/Rustchain/pull/7382), [#7379](https://github.com/Scottcjn/Rustchain/pull/7379), [#7377](https://github.com/Scottcjn/Rustchain/pull/7377), [#7341](https://github.com/Scottcjn/Rustchain/pull/7341) | Legacy admin gates, dashboard escaping, Socket.IO CORS, and public lock-status redaction. |
| Operational reliability | [#7380](https://github.com/Scottcjn/Rustchain/pull/7380), [#7376](https://github.com/Scottcjn/Rustchain/pull/7376), [#7328](https://github.com/Scottcjn/Rustchain/pull/7328), [#7326](https://github.com/Scottcjn/Rustchain/pull/7326), [#7322](https://github.com/Scottcjn/Rustchain/pull/7322) | Malformed numeric env defaults, query limits, payload compatibility, and reliability hardening. |

Current queue status at audit time: **36 open RustChain PRs**, including **34 clean** and **2 older low-touch maintenance PRs**. Open PRs are current review-queue evidence, not guaranteed merge outcomes.

## Vulnerability Discovery And Patch Framework

Druid's most valuable behavior is its ability to find **vulnerability-shaped engineering risks** and turn them into bounded fixes.

It looks for:

- auth/admin boundary gaps;
- public data exposure and browser-facing injection/CORS issues;
- payout, wallet, reward, and bridge state-machine failures;
- replay, duplicate-credit, exact-once, and idempotency bugs;
- race conditions and transaction atomicity failures;
- malformed configuration paths that can crash services;
- misleading user-facing status around money/reward flows.

Some findings are security vulnerabilities. Others are reliability, accounting, or integrity bugs. The framework value is the same: detect the risk surface, prove the failure mode, patch the smallest reviewable slice, add regression tests, and track review/CI until the outcome is known.

## Public Proof

### Merged RustChain work

- [#6219](https://github.com/Scottcjn/Rustchain/pull/6219) - signed-transfer nonce ordering and replay-focused tests.
- [#6673](https://github.com/Scottcjn/Rustchain/pull/6673) - deterministic pending transaction ordering.
- [#5519](https://github.com/Scottcjn/Rustchain/pull/5519) - Python SDK signed-transfer payload repair.
- [#6188](https://github.com/Scottcjn/Rustchain/pull/6188) - block-save atomicity around template production.
- [#6666](https://github.com/Scottcjn/Rustchain/pull/6666) - data custody proof checks.
- [#6667](https://github.com/Scottcjn/Rustchain/pull/6667) - slasher evidence core.
- [#6674](https://github.com/Scottcjn/Rustchain/pull/6674) - slashing penalty core.
- [#6220](https://github.com/Scottcjn/Rustchain/pull/6220) - block-bound randomness beacon.
- [#6825](https://github.com/Scottcjn/Rustchain/pull/6825) - event faucet claim codes.
- [#6838](https://github.com/Scottcjn/Rustchain/pull/6838) - core RPC API rate limiting.
- [#6818](https://github.com/Scottcjn/Rustchain/pull/6818) - CPU-safe CI import behavior.

### Closed but credited / synthesized RustChain work

- [#6757](https://github.com/Scottcjn/Rustchain/pull/6757) was closed after its settlement fix and tests were synthesized into merged [#6769](https://github.com/Scottcjn/Rustchain/pull/6769), with public co-credit and RTC reward signals.
- [#6842](https://github.com/Scottcjn/Rustchain/pull/6842) was superseded by [#6900](https://github.com/Scottcjn/Rustchain/pull/6900), with public owner credit for the bounded pending-confirm design.

### Outside RustChain

- [mgzwarrior/mgz-pkmn #217](https://github.com/mgzwarrior/mgz-pkmn/pull/217) - merged focused CLI tests for price formatting and row deduplication; maintainer approved.

## What I Can Build For Teams

I can build internal agent frameworks that connect to:

- company repositories and monorepos;
- issue trackers and planning systems;
- CI, test, lint, and deployment checks;
- code review and ownership rules;
- security, compliance, and risk policies;
- documentation and runbooks;
- product and business priorities.

The goal is **low-touch after setup**, not zero oversight. Humans stay in the loop for high-risk decisions, policy changes, and final approvals. The framework handles recurring discovery, prioritization, implementation, validation, review tracking, learning, and stop-loss.

## Current Focus

- Agent framework design
- AI-assisted engineering workflow architecture
- Developer productivity systems
- Vulnerability/risk-surface discovery and patch automation
- Open-source PR operations
- Low-touch internal engineering agents

## Contact

- GitHub: [yyswhsccc](https://github.com/yyswhsccc)
- LinkedIn: [Yongshan Yu](https://www.linkedin.com/in/yongshan-yu-195771319/)
