# plori extension for Gemini CLI

Create and drive AI agents in persistent cloud environments. This extension connects
[Gemini CLI](https://github.com/google-gemini/gemini-cli) to
[plori](https://plori.ai)'s remote MCP server so you can create and drive hosted
agents with durable disk, real tools, and memory from your terminal.

## Install

```sh
gemini extensions install https://github.com/plori-ai/gemini-extension
```

There is nothing else to run locally: the MCP server is hosted at
`https://api.plori.ai/mcp`. On first use you sign in with your email in the browser
(one-time code, no password).

## Try it

```
> List my plori agents and show my current balance.
> Create an agent called scout and ask it to summarize the top HN story.
```

The extension exposes the current 25-tool surface for agents, runs, human input,
scheduling, connections, workflows, and account state. Creating and invoking agents
spends your prepaid balance; read-only tools are free. Details:
[plori.ai/pricing](https://plori.ai/pricing).

## Links

- Connect guide for every client: [plori.ai/mcp](https://plori.ai/mcp)
- For AI agents: [plori.ai/agents.md](https://plori.ai/agents.md)
- Privacy: [plori.ai/privacy](https://plori.ai/privacy) · Terms: [plori.ai/terms](https://plori.ai/terms)
- Questions: [dev@plori.ai](mailto:dev@plori.ai)
