# Talk slides — Building a Conversational Sales Agent with LangChain & MCP

A single-file HTML slide deck (style modeled on
[marlenezw/agentic-coding-talk](https://github.com/marlenezw/agentic-coding-talk))
for the talk:

> Build a conversational AI agent that analyzes sales data and helps customers
> find products — using **LangChain**, **Model Context Protocol (MCP)**,
> **PostgreSQL with RLS + pgvector**, and the **OpenAI Responses API** built-in
> tools (image generation, code interpreter, web search).

The deck is based on the code in this repo
([`Azure-Samples/langchain-agent-python`](https://github.com/Azure-Samples/langchain-agent-python))
and on the [AI Tour WRK540 workshop guide](https://microsoft.github.io/aitour26-WRK540-unlock-your-agents-potential-with-model-context-protocol/).

## Run it

It's a single static file — open it in any modern browser:

```bash
open slides/index.html
# or
python -m http.server -d slides 8080   # then visit http://localhost:8080
```

## Navigate

- `→` / `Space` / click right half → next slide
- `←` / click left half → previous slide
- `Home` / `End` → first / last slide

## Outline

1. Title
2. Hi, I'm Marlene
3. Agenda
4. Section — *Why LangChain?*
5. Azure × LangChain (tweet)
6. What is LangChain?
7. Who's building with LangChain (Fin, LinkedIn, Harvey)
8. Section — *The app we'll build*
9. Meet Zava
10. Architecture
11. Section — *What is an AI agent?*
12. An agent is a loop
13. The agentic loop diagram
14. Section — *What is MCP?*
15. MCP excalidraw
16. Loop zoom — **Gather Context**
17. Context · MCP & Postgres tools
18. Security · Postgres RLS
19. Context engineering — refine / summarize / validate
20. LangChain code — gathering context
21. Loop zoom — **Take Action**
22. Tools you don't have to build (code, web, image)
23. Built-in tools, in code
24. `apply_step_config` — splitting prompts & tools per step
25. Loop zoom — **Validate**
26. Validation — traces, grounding, evals, monitoring
27. Resources
28. Thank you

## Editing

Everything (HTML, CSS, JS, content) lives in `slides/index.html`. Tweak copy
in the `<div class="slide">` blocks and it just works — no build step.
