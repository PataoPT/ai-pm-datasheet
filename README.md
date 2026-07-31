# The AI PM Datasheet

A self-contained course on how AI products actually work — from zero, assuming no
machine-learning background. Not a glossary and not a listicle: nine mental models,
taught mechanism-first, that let you reason about systems you have never seen.

Written by [Diogo Patão](https://www.linkedin.com/in/diogopatao/) — Chief of Staff
at Stake Capital Group, GM at Rekt News, and founder of
[10Q Capital](https://10q.capital). Free, no signup, no tracking.

**Live:** <https://ai-pm-datasheet.vercel.app>

## What it is

One HTML file. No build step, no dependencies, no external requests — open
`index.html` in any browser, online or offline, and it works.

- **9 chapters** in dependency order, each assuming the last: how an LLM actually
  works (tokens, embeddings, next-token prediction, transformers, attention) →
  sampling and the context window → hallucination and grounding → RAG and context
  engineering → tools, agents and MCP → orchestration and routing → evals and
  metrics → system design and trade-offs → the interview itself.
- **53 diagrams**, hand-authored as inline SVG, themed for light and dark.
- **6 interactive labs** — a tokenizer, an attention explorer, a temperature and
  sampling lab with real softmax, a context-window budget allocator, a
  precision/recall threshold lab, and an inference cost and chain-reliability
  model.
- **90 worked answers** to the real questions people ask about each topic.
- A **searchable question index**, a **58-question self-test**, and a **printable
  cheat sheet** with an 89-term glossary.

## On the numbers

Every calculation in the labs is exact: the softmax, the confusion matrix, the
cost arithmetic. Two labs are deliberately labelled as approximations in their own
footers — the tokenizer applies simple rules rather than a real learned vocabulary,
and the attention weights are hand-specified to illustrate what heads are observed
to do rather than measured from a live model.

Any figure for token pricing, latency, or model capability is an illustrative
order of magnitude and will go out of date. The reasoning is the durable part, not
the number. Verify specifics against current provider documentation before quoting
them anywhere that matters.

## Credit

The ~110 questions used to structure the site come from the "Technical AI PM
Interview Questions" sheet compiled by **Aakash Gupta** (news.aakashg.com) — a good
map of what people actually need to understand about AI products, which is what made
it a good syllabus. The questions are his; the explanations, diagrams, interactive
labs, and worked answers here are original.

## Local use

```
open index.html
```

That's it. It is one file and it has no dependencies.
