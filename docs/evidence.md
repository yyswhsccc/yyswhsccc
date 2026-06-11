# Druid Public Evidence

Last audited: **2026-06-11**.

All counts below were checked with live GitHub queries. Open PRs are review-queue
evidence, not merged or rewarded claims.

## Counts

| Scope | Count |
|---|---:|
| Merged PRs authored by `yyswhsccc`, all repositories | 47 |
| Merged PRs authored by `yyswhsccc` in `Scottcjn/Rustchain` | 45 |
| Open PRs authored by `yyswhsccc` in `Scottcjn/Rustchain` | 36 |

## Selected Merged Proof

| PR | Status | Proof value |
|---|---|---|
| [RustChain #6219](https://github.com/Scottcjn/Rustchain/pull/6219) | Merged | Signed-transfer nonce ordering with replay-focused tests. |
| [RustChain #6188](https://github.com/Scottcjn/Rustchain/pull/6188) | Merged | Block-save atomicity around template production. |
| [RustChain #6667](https://github.com/Scottcjn/Rustchain/pull/6667) | Merged | Slasher evidence core for security economics work. |
| [RustChain #6838](https://github.com/Scottcjn/Rustchain/pull/6838) | Merged | Core RPC API rate limiting. |
| [RustChain #6757](https://github.com/Scottcjn/Rustchain/pull/6757) -> [#6769](https://github.com/Scottcjn/Rustchain/pull/6769) | Superseded into merged synthesis | Maintainer-synthesized settlement guard work. |
| [mgz-pkmn #217](https://github.com/mgzwarrior/mgz-pkmn/pull/217) | Merged | Transfer beyond RustChain into maintainer-approved CLI helper tests. |

## RustChain Open Review Queue

### Payout Exact-Once / Terminal Status

- [#7385](https://github.com/Scottcjn/Rustchain/pull/7385) — missing payout status rows return 404.
- [#7378](https://github.com/Scottcjn/Rustchain/pull/7378) — tip-bot decimal precision validation.
- [#7357](https://github.com/Scottcjn/Rustchain/pull/7357) — ledger terminal status guard.
- [#7355](https://github.com/Scottcjn/Rustchain/pull/7355) — remaining-balance withdraw gauge.
- [#7353](https://github.com/Scottcjn/Rustchain/pull/7353) — pending withdrawals claimed once.

### Bridge Terminal Integrity

- [#7363](https://github.com/Scottcjn/Rustchain/pull/7363) — report bridge last state change time.
- [#7343](https://github.com/Scottcjn/Rustchain/pull/7343) — guard void against terminal races.
- [#7330](https://github.com/Scottcjn/Rustchain/pull/7330) — tolerate malformed bridge config env.
- [#7316](https://github.com/Scottcjn/Rustchain/pull/7316) — clarify operator-only bridge initiate flow.

### UTXO / Transaction Atomicity

- [#7350](https://github.com/Scottcjn/Rustchain/pull/7350) — serialize pending nonce admission.
- [#7339](https://github.com/Scottcjn/Rustchain/pull/7339) — single-source apply transaction ownership flag.
- [#7337](https://github.com/Scottcjn/Rustchain/pull/7337) — expose absorbed coin selection fee.
- [#7336](https://github.com/Scottcjn/Rustchain/pull/7336) — bound box id output index encoding.
- [#7335](https://github.com/Scottcjn/Rustchain/pull/7335) — align mempool value sum with unspent inputs.
- [#7334](https://github.com/Scottcjn/Rustchain/pull/7334) — preserve external transaction ownership.
- [#7333](https://github.com/Scottcjn/Rustchain/pull/7333) — roll back invalid mempool timestamps.

### Governance Accounting

- [#7347](https://github.com/Scottcjn/Rustchain/pull/7347) — paginate API proposal votes.
- [#7345](https://github.com/Scottcjn/Rustchain/pull/7345) — avoid charging rejected proposals.

### Bounty Attribution / Claims

- [#7383](https://github.com/Scottcjn/Rustchain/pull/7383) — report keeper claims as receipts.
- [#7367](https://github.com/Scottcjn/Rustchain/pull/7367) — return false for missing claim status rows.
- [#7361](https://github.com/Scottcjn/Rustchain/pull/7361) — require claimed bounty completion.
- [#7359](https://github.com/Scottcjn/Rustchain/pull/7359) — persist bounty claims.

### Browser / Security Boundaries

- [#7382](https://github.com/Scottcjn/Rustchain/pull/7382) — gate legacy protocol escrow routes.
- [#7379](https://github.com/Scottcjn/Rustchain/pull/7379) — escape dashboard status fields.
- [#7377](https://github.com/Scottcjn/Rustchain/pull/7377) — restrict Socket.IO CORS origins.
- [#7341](https://github.com/Scottcjn/Rustchain/pull/7341) — redact public bridge lock status.

### Operational Reliability

- [#7380](https://github.com/Scottcjn/Rustchain/pull/7380) — tolerate malformed PoA numeric env defaults.
- [#7376](https://github.com/Scottcjn/Rustchain/pull/7376) — tolerate malformed rate-limit env defaults.
- [#7365](https://github.com/Scottcjn/Rustchain/pull/7365) — floor lock helper query limits.
- [#7328](https://github.com/Scottcjn/Rustchain/pull/7328) — tolerate malformed epoch settler env.
- [#7326](https://github.com/Scottcjn/Rustchain/pull/7326) — tolerate malformed webhook numeric env.
- [#7324](https://github.com/Scottcjn/Rustchain/pull/7324) — tolerate malformed alerts numeric env.
- [#7322](https://github.com/Scottcjn/Rustchain/pull/7322) — tolerate malformed Prometheus numeric env.
- [#7320](https://github.com/Scottcjn/Rustchain/pull/7320) — unwrap paginated miners payload.

### Older Low-Touch Maintenance

- [#6823](https://github.com/Scottcjn/Rustchain/pull/6823) — miner header key rotations.
- [#6182](https://github.com/Scottcjn/Rustchain/pull/6182) — pending tx nonce admission.
