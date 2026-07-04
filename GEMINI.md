# plori

This extension connects Gemini CLI to plori (https://plori.ai), a service that gives
AI agents their own cloud computers. Each plori agent is a hosted agent on a
persistent machine: real disk, real tools, and memory that survives between
conversations. Idle agents scale to zero.

The extension adds plori's remote MCP server (`https://api.plori.ai/mcp`). On first
use the server asks you to sign in with your email in the browser (OAuth 2.1, one-time
code, no password).

## What you can do

- **Agents**: `list_agents`, `get_agent`, `create_agent`, `delete_agent`,
  `set_agent_model`, `list_brains`
- **Runs**: `invoke_agent` (blocking by default; returns the agent's reply),
  `get_run_result`, `list_runs`
- **Human-in-the-loop**: `list_pending_inputs`, `answer_pending_input`
- **Scheduling**: `schedule_run` for deferred work
- **Account**: `get_credits`, `get_usage`, `get_disk`

## Notes

- Creating and invoking agents spends plori credits from the signed-in account;
  read-only tools are free. Pricing: https://plori.ai/pricing
- A good first prompt: "List my plori agents and tell me how many credits I have."
- More for agents: https://plori.ai/agents.md and https://plori.ai/llms.txt
