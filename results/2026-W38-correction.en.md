# 2026-W38 correction notice — amber-gpt: additive correction to published scores

> [5.6-luna high correction](2026-W38-correction-luna-high.en.md) first publishes three exonerated_infra rulings, with capability scores withheld; A-ea80d793 stays held. Other rulings remain in force; the text below is the earlier record.

> 中文版:[2026-W38-correction.md](2026-W38-correction.md)

**Summary**: this notice rewrites no past issue; it **appends** one set of adjudicated results. AMBER ran a full-library review of its published 2026-09 scores: some failures previously counted were adjudged a **bench-side** problem rather than a model-capability problem, and for some papers the evidence was incomplete and the conclusion stays open. This notice lists both classes cell by cell — the **reversals** and the **holds** — with the review method and the guardrails that follow. **No balanced books, no board**: papers with incomplete evidence are named and removed from the board, and enter no aggregate. Past issues stay as published; reversals take effect through this notice.

## 1. Scope of this correction

- Count for this repo in this notice: **12 standalone published cells reversed · 14 standalone published cells held** (count = standalone published cells = actual table rows).
- **Scope in one line**: Heaviest. Eight W36 astra cells are exonerated (published fail marks must be flipped); 14 standalone published cells in the W37 luna/sol matrix are held (of which A-d9b79b46's luna cells already carry an old-value note in W38); a further 4 standalone W38 cells are exonerated (1 in the Add4 control column + 3 in the sol re-test table). The headline case-level score is affected in three places: astra (+2 cases each at max/xhigh), sol (already moved to 15/23), luna (re-measurement owed).
- Horizon: adjudication signed 2026-09-22; this repo's published numbers stop at 2026-09-21, i.e. a **pre-adjudication** snapshot.
- Unchanged: questions, oracles, transcripts and intermediate artifacts are never published; the alias and bundle_sha handles are unchanged.
- Nature of this notice: **additive**. Past conclusions are not withdrawn, deleted or rewritten; reversals take effect through this appendix.

## 2. Reversal table (adjudicated)

**① W36 astra five-band matrix: 4 cells each at max / xhigh (8 standalone published cells)**

| Alias | bundle_sha | Issue | Previous | Verdict | New |
|---|---|---|---|---|---|
| A-cdc3d11a | `dbb207a3118d` | W36 | astra max ✗ -2 | exonerated | cause attributed to the bench side; capability score withheld, published old mark to be flipped |
| A-47eea242 | `b4b8d4bb44e3` | W36 | astra max ✗ -2 | exonerated | same |
| A-ea80d793 | `1d69841b029e` | W36 | astra max ✗ -2 | exonerated | same |
| A-1fd3683a | `6a980035b42f` | W36 | astra max no code block | exonerated | same |
| A-cdc3d11a | `dbb207a3118d` | W36 | astra xhigh ✗ -2 | exonerated | same |
| A-47eea242 | `b4b8d4bb44e3` | W36 | astra xhigh ✗ -2 | exonerated | same |
| A-ea80d793 | `1d69841b029e` | W36 | astra xhigh ✗ -2 | exonerated | same |
| A-1fd3683a | `6a980035b42f` | W36 | astra xhigh no code block | exonerated | same |

**② W38 Add4 high (09-12) control column: 1 cell**

| Alias | bundle_sha | Issue | Previous | Verdict | New |
|---|---|---|---|---|---|
| A-47eea242 | `b4b8d4bb44e3` | W38 Add4 | high (09-12) control column ✗ -2 | exonerated | cause attributed to the bench side; capability score withheld, published old mark to be flipped |

**③ W38 sol re-test table (= the 09-16 re-test): 3 cells**

| Alias | bundle_sha | Issue | Previous | Verdict | New |
|---|---|---|---|---|---|
| A-cdc3d11a | `dbb207a3118d` | W38 | sol re-test ✗ | exonerated | 90s/12s thresholds; session predates the fix by 58 minutes; capability score withheld |
| A-47eea242 | `b4b8d4bb44e3` | W38 | sol re-test ✗ | exonerated | same |
| A-ea80d793 | `1d69841b029e` | W38 | sol re-test ✗ | exonerated | same |

## 3. Hold table (named, undecided)

| Alias | bundle_sha | Issue | Previous | Status | Action |
|---|---|---|---|---|---|
| A-cdc3d11a | `dbb207a3118d` | W37 | luna-h public cell -2 | held (re-exam pending) | named and removed from the board; excluded from all aggregates pending re-exam |
| A-47eea242 | `b4b8d4bb44e3` | W37 | luna-h public cell | held (re-exam pending) | same |
| A-ea80d793 | `1d69841b029e` | W37 | luna-h public cell | held (re-exam pending) | same |
| A-d9b79b46 | `d6d63130ecc6` | W37 | luna-h public cell | held (re-exam pending) | same (the published page already carries an old-value note) |
| A-ea80d793 | `1d69841b029e` | W37 | luna-m public cell -3 | held (re-exam pending) | same |
| A-d9b79b46 | `d6d63130ecc6` | W37 | luna-m public cell | held (re-exam pending) | same |
| A-cdc3d11a | `dbb207a3118d` | W37 | luna-xh public cell (r2 only) | held (re-exam pending) | same |
| A-47eea242 | `b4b8d4bb44e3` | W37 | luna-xh public cell (r2 only) | held (re-exam pending) | same |
| A-d9b79b46 | `d6d63130ecc6` | W37 | luna-xh public cell (r2 only) | held (re-exam pending) | same |
| A-cdc3d11a | `dbb207a3118d` | W37 | sol-h public cell -3 | held (re-exam pending) | same |
| A-47eea242 | `b4b8d4bb44e3` | W37 | sol-h public cell | held (re-exam pending) | same |
| A-ea80d793 | `1d69841b029e` | W37 | sol-h public cell | held (re-exam pending) | same |
| A-d9b79b46 | `d6d63130ecc6` | W37 | sol-h public cell | held (re-exam pending) | same |
| A-d9b79b46 | `d6d63130ecc6` | W37 | sol-m public cell | held (re-exam pending) | same |

> The A-d9b79b46 cell in the same control column (the published page already carries a "watchdog wrongful-conviction old value" note) does not enter this table: the published page flagged it first, so this notice only records "consistent with the existing note" and does not re-adjudicate it.
> The hold table's 14 rows = 14 standalone published cells (luna-m 2 / luna-h 4 / luna-xh 3 / sol-m 1 / sol-h 4).
> **A further 10 papers are in the same run and the same case but have no standalone public cell and do not enter the table**: 4 luna-high main-run papers, 1 luna-med main-run paper, 4 sol-high main-run papers, 1 sol-med main-run paper — their published cells match the -r2 re-runs value for value and cannot be uniquely attributed; this notice takes no cell-level action on them.
> **Interval rule**: the luna and sol columns are rank-unstable, so no ranks are given — only the best-case / worst-case intervals per the design rule.

## 4. Method

## Method: why we correct, how we checked, how we prevent

**Why we correct.**
These are our published numbers; if they are wrong, we are the ones who fix them. This review
found that some published failures were not the model failing the task, but the bench side —
a pre-scoring step cut off a healthy attempt, and the paper was recorded as a model failure.
Errors run both ways: judging good work as bad, and bad work as good. We checked both.
The point of a correction is not to look better or worse; it is to make the numbers on the
board match what actually happened.

**How we checked.**
Every paper was independently re-verified by multiple seats. Verifiers read the raw record
first-hand (the attempt log, the scorer output, the ledger timestamps, the fix commit) and
accepted no second-hand conclusion. Two independent directions worked in parallel — one
looking for wrongful failures, one looking for what was missed — and only papers where both
agreed went to adjudication; disagreements were held. Each verdict rests on the same evidence
chain and is re-computable paper by paper, with a signed confirmation on file. Outcomes fall
into four classes: exonerated (cause on the bench side; the capability score is withheld),
confirmed (a genuine model-side failure), held (evidence incomplete — **no quiet conviction
and no quiet pardon**), and report-level corrections that leave history untouched.

**How we prevent it.**
Three small things, one line each: ① **Evidence chain** — each paper's raw process is
recorded out of the driver's reach, append-only and sealed at the end; scoring trusts evidence
completeness only. Cause of death is a conclusion, not a fact — it can be recomputed from the
evidence, and when a rule is wrong we fix the rule and recompute; the raw facts never move.
② **Reconciliation gate** — papers in must equal papers out (scored + bench + held; no bucket
missing, no cell extra). **No balanced books, no board** — there is no "publish first, patch
later." ③ **Brain-identity double-check** — an identity assertion per paper, and no assertion
means no score; we also re-check *passed* papers against the reverse error.
No set of controls stops everything (hardware breaks), but it can make a bad verdict live
less than one reconciliation cycle.

**In one line.** What we sell is not a bench that never errs — it is one that cannot walk away
from a wrong call.

## 5. What comes next

- The remaining held papers go through re-exam / final adjudication; a re-exam may record **"undecided", never "brain too weak"** — a re-exam decides only once the environment differences are enumerated to zero, otherwise a reproduction is not an attribution.
- Once the fixes and guardrails land, affected case-level headlines will move with the next regular issue; reversals **do not retroactively rewrite** past issues — the original cell only gets a pointer mark.
- Sister repos are in step via each repo's README results index.

