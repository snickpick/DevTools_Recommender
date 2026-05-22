# Developer Tools Recommender

LangGraph agent that searches, researches, and recommends developer tools for a given scenario.

## Features

- **3-node LangGraph workflow** — extract tools from search, research each one, generate a recommendation
- **Firecrawl search + scrape** — pulls live web data for any developer tool query
- **Structured LLM analysis** — extracts pricing, open-source status, tech stack, API availability, language support, and integrations via Pydantic models
- **OpenRouter LLM** — uses ring-2.6-1t:free for inference

## Setup

```sh
uv sync
```

Create `.env`:

```
FIRECRAWL_API_KEY=your_key
OPENROUTER_API_KEY=your_key
```

## Run

```sh
uv run python main.py
```

Enter a query like "serverless database" or "React form library" at the prompt.
