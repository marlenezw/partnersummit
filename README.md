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
2. Agenda
3. Section — *Meet Zava*
4. The problem (customers, managers, security)
5. What we're building
6. Section — *Agents, briefly*
7. An agent is a loop
8. LangChain `create_agent` code
9. Section — *Model Context Protocol*
10. Why MCP
11. The three primitives (tools / resources / prompts)
12. Our FastMCP server (the 4 real tools from `mcp/app.py`)
13. Section — *One database, two superpowers*
14. Row Level Security
15. pgvector
16. Section — *Responses API*
17. Built-in tools (image / code / web)
18. Turning them on
19. Section — *Putting it all together*
20. Architecture diagram
21. End-to-end question flow
22. Section — *Demo*
23. Run it locally
24. The system prompt is half the agent
25. Section — *Ship it*
26. `azd up`
27. Takeaways
28. Thank you + resources

## Editing

Everything (HTML, CSS, JS, content) lives in `slides/index.html`. Tweak copy
in the `<div class="slide">` blocks and it just works — no build step.
