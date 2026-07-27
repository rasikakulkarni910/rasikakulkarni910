# Rasika Kulkarni

**AI Solutions Architect · Mountain View, CA · Open to remote roles**

I design and ship enterprise AI systems — retrieval-augmented generation,
tool-using agents, and the evaluation infrastructure that makes them
defensible to a customer's security and finance teams.

I care about the parts most AI demos skip: what the system costs per query,
what its P95 latency is, what it does when retrieval fails, and how you prove
quality did not regress after a prompt change.

**Currently:** building reference architectures for teams adopting LLMs in
regulated, multi-tenant environments.

**Recent outcomes:** 94% task accuracy and 71% containment on a production
assistant · P95 latency held at 2.2s · reduced AI proof-of-value delivery from
eight weeks to two · six-figure annual customer savings.

**Stack:** Python · TypeScript · SQL · Vertex AI · Gemini · Cloud Run ·
BigQuery · Terraform · Docker


---

## What I work on

Most enterprise RAG systems fail in the same few places: retrieval quality
nobody measured, prompt changes nobody regression-tested, and a cost curve
nobody modeled until the invoice arrived. These repositories are where I work
through those problems and write down what I find — including the parts that
still don't work.

Four things I've come to believe, and where each is argued:

**Retrieval quality is the ceiling on answer quality.** No amount of prompt
engineering recovers from a bad chunk. Measured recall@k and nDCG@k across a
100-question labeled set, plus the five retrieval failures I haven't solved —
[evals/RESULTS.md](link)

**An LLM is often the wrong component for the job.** In the migration control
tower, deterministic rules handle the clear cases and a model reviews only the
ambiguous ones. I measured whether that split was actually correct rather than
assuming it — [docs/RULES_VS_LLM.md](link)

**Agent permissions are a design problem, not a prompt problem.** Tool
allow-lists, mandatory human approval on side-effecting calls, and a
prompt-injection suite the system has to pass before anything merges —
[docs/THREAT_MODEL.md](link)

**Latency and cost are architecture decisions, not later optimizations.**
Cost per thousand queries, P50 and P95, and what quality you actually give up
moving between model tiers — [docs/COST_LATENCY.md](link)

How the whole system fits together: [docs/ARCHITECTURE.md](link).
If you'd rather watch it run: [90-second walkthrough](link).

Rasika Kulkarni — Mountain View, CA, open to remote.
[Email](mailto:) · [LinkedIn](link) · [Résumé](link)

---
