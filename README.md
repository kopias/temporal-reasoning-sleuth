# Temporal Reasoning Sleuth

**A Claude Code skill — engineer temporal reasoning so an agent can trace decision chains and reconstruct causal sequences across months or years of history.**

> "What decisions led to X?" breaks plain RAG. This skill is the **read/query
> path**: event graphs, causal-chain traversal, and windowed context synthesis
> that feed the model a curated causal slice instead of a raw timeline dump.

---

## What it does

Engineers temporal reasoning for AI agents: the three temporal query types
(sequence / causal / counterfactual), event-graph + causal-chain-index +
windowed-synthesis patterns, and the workflow to answer a causal query.

## When to use it

When an agent must answer "what led to X", "how did this evolve", or any query
needing temporal sequencing and causation across many events.

## When NOT to use

- You need to **capture/ingest** institutional events or define the storage
  schema (the write path) → use [`synthesizing-institutional-knowledge`](https://github.com/kopias/synthesizing-institutional-knowledge).
- You're choosing between retrieval paradigms → use [`designing-hybrid-context-layers`](https://github.com/kopias/designing-hybrid-context-layers).

## Related skills

- [`synthesizing-institutional-knowledge`](https://github.com/kopias/synthesizing-institutional-knowledge) — the write-path counterpart (capture/schema)
- [`designing-hybrid-context-layers`](https://github.com/kopias/designing-hybrid-context-layers) — the umbrella architecture this is Layer 3 of
- [`diagnosing-rag-failure-modes`](https://github.com/kopias/diagnosing-rag-failure-modes) — why RAG fails on temporal/causal queries

## Install

The skill lives in the [`temporal-reasoning-sleuth/`](temporal-reasoning-sleuth)
folder (this README is for humans and is **not** part of the skill).

```bash
git clone https://github.com/kopias/temporal-reasoning-sleuth.git
cp -r temporal-reasoning-sleuth/temporal-reasoning-sleuth ~/.claude/skills/
```

Claude Code picks the skill up automatically on relevant tasks.
