# Module 1 — Agentic RAG (Homework)

Solution notebook: [`homework.ipynb`](homework.ipynb).

Built a RAG system over the course **lessons** (pulled from the course repo at commit
`8c1834d`), then turned it into an agent that decides when to search.

LLM used: **Claude `claude-haiku-4-5`** (Anthropic). The homework allows any provider,
so the token/agent numbers are the "closest option".

## Answers

| Question | Answer |
|---|---|
| Q1 — lesson pages | 72 |
| Q2 — top search result | `01-agentic-rag/lessons/14-agentic-loop.md` |
| Q3 — RAG input tokens | 7000 |
| Q4 — chunks (size=2000, step=1000) | 295 |
| Q5 — token reduction with chunking | 3× fewer |
| Q6 — agent `search` calls | 4 |

## Run it

```bash
uv add gitsource minsearch anthropic
export ANTHROPIC_API_KEY=...   # not stored in the repo
jupyter notebook homework.ipynb
```

The API key is read from the environment (`anthropic.Anthropic()`); it is never
hard-coded in the notebook.
