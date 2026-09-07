# amber-gpt

Weekly public benchmark results of GPT-family models (across reasoning-effort bands) on the private **AMBER** suite — cases private, results public.
中文: [README.md](README.md)

## What this is

- One issue per week at `results/YYYY-Www.md`: same cases, same harness, full library; the same model at different effort bands side by side.
- Every issue reports: case-set size and hashes, per-case d2 scores and pass/fail, terminal states, token usage and latency, environment fingerprint, and qualitative verdicts written under evidence discipline.
- Cases, oracles, transcripts, and intermediate artifacts are **never published** (see "Publication discipline").
- Sister repos: [amber-crof](https://github.com/getaskclaw/amber-crof) (CrofAI weekly), [amber-ollama](https://github.com/getaskclaw/amber-ollama) (Ollama Cloud weekly).
- The AMBER suite spec and case-authoring tools live at [getaskclaw/amber-eval](https://github.com/getaskclaw/amber-eval); the case contents themselves are private.

## Publication discipline (red lines)

1. Publish only: scores and aggregates, token usage, latency, qualitative verdicts.
2. Never publish: case content, oracles/graders, transcripts, candidate workspaces, or any intermediate artifact that could reconstruct a case.
3. Every issue pins: model ID, effort band, date (UTC), harness version, and per-case content hashes (bundle_sha). Hashes line up with the public hash manifest in [amber-eval](https://github.com/getaskclaw/amber-eval) so anyone can verify the case set has not changed.
4. Case IDs and case structure are private: public results refer to cases only by stable aliases (A-xxxxxxxx, hash-derived) plus bundle hashes; internal case IDs, variant names, and case descriptions never appear.
5. Tone: this is a community weekly measurement, not an attack on any vendor. Let the data talk; keep wording restrained.

## A methodological premise

The same model on the same provider can score differently across runs — serving versions, load, and parameters drift. Everything here carries a date and an effort band, and is re-measured weekly. A single day's number is a snapshot, not a law.

## Results index

| Issue | Content | Verdict |
|---|---|---|
| (first issue in preparation) | — | — |

## Disclaimer

Not affiliated with or sponsored by OpenAI. Scores are snapshots of a specific week and effort band — not procurement advice.
