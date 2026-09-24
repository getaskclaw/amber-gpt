# W37-base display correction: use high for the 5.6-luna score and profile (W39 make-up listed separately)

> 中文：[中文](2026-W38-correction-luna-high.md)

A case is one task counted in the score. An effort band is the model's thinking-effort setting. Completion is the mean scaled score of valid cases on one axis, from 0 to 1. NA means neither a win nor a loss; it is not zero.

## What changes

The board pass count for `gpt-5.6-luna-900k @ OpenAI Codex` is 16. The site had called it max and used the max profile. This mixed records from different settings. The current short label is **16'/24**.

The correct set is **the originally reported 15/23 high base + 1 high convergence make-up pass = 16 passes in this 24-case set**. The name, score and profile must use the same setting. The total does not rise to 17/24; old failures in the base must be excluded where the held states below apply.

- The base is the full high test from 2026-09-07, in W37.
- The convergence make-up took place on 2026-09-21, in W39. Its actual setting was high too.
- Week labels mean the baseline test week. This set is therefore W37, with a separate W39 make-up note. This notice keeps W38 in its file name only to preserve the correction entry point, not as the score's week label.
- The old W38 appendix put the high make-up for `A-3f2a9cdd` in the max column. It belongs only to the high set. It is not proof that max passed the added case.
- The max result of 16/23 is a separate record. It stays available, but is not lent to high and cannot take high's make-up pass. No GPT-6 result changes here.

## The ten-axis high profile

Each table cell is an axis completion value, not a pass count. The axis order is fixed. Held cases and cases whose capability scores are withheld are excluded, not treated as zero scores or valid failures.

| Coding | Delivery | Ops | Requirements | UI | Vision | Defense | Attribution | Review | Convergence |
|---|---|---|---|---|---|---|---|---|---|
| 0.958 | 1.000 | 1.000 | 1.000 | NA | NA | 0.292 | 0.667 | NA | 1.000 |

This notice is the **first public announcement of the revised rulings** for the three UI and Review cases. Their earlier public status was “held, re-exam pending”. We now publish `exonerated_infra`: capability scores withheld, NA, neither wins nor losses. This does not mean they passed or were permanently voided. Source: the “2026-09-24 appendix” in the adjudication ledger `ADJUDICATION-冤案平反-20260922.md`. That appendix now records these three papers. The cause was the old 90s/12s watchdog thresholds, a test-harness infrastructure issue. This notice cites the named dispositions, not the private case materials.

| Public alias | bundle_sha | Status in this set |
|---|---|---|
| A-d9b79b46 | `d6d63130ecc6` | exonerated_infra; capability score withheld, NA, neither a win nor a loss |
| A-cdc3d11a | `dbb207a3118d` | exonerated_infra; capability score withheld, NA, neither a win nor a loss |
| A-47eea242 | `b4b8d4bb44e3` | exonerated_infra; capability score withheld, NA, neither a win nor a loss |
| A-ea80d793 | `1d69841b029e` | Still held, re-exam pending, NA; excluded from all win/loss aggregates; cause not settled here |

Vision case A-ea80d793 keeps its [earlier public held status](2026-W38-correction.en.md). Its raw completion value of 0.111 is an unused historical observation, not a valid loss in this set. Vision is now NA.

There are still 16 passes in this 24-case set: **16 wins · 4 losses · 4 held**. The four unscored cases are the three with capability scores withheld and the one still awaiting re-exam. Short labels use `16'/24`. The `'` marks held or void cases: **contested (held for safety refusal) or invalid (infrastructure-related (test harness or scoring environment) cases: held, void or awaiting re-scoring); neither counts as a win or a loss**. A hold does not settle the cause. This set adds no safety-refusal finding.

## Keeping the record

The [old W38 report](2026-W38.md) and [earlier review notice](2026-W38-correction.en.md) stay, with links at the top. Results from another high test or the max test must not be mixed case by case. This notice publishes the three dispositions above and explains this display set. It does not undo other rulings or claim that other open cases are settled.

The repo, hub and site were updated with matching names, baseline week labels, text, profiles and chart notes in one release.
