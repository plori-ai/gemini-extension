# plori

This extension connects Gemini CLI to plori (https://plori.ai). Each plori agent runs
in its own persistent cloud environment with a durable disk, a shell, developer tools,
and memory.

The extension adds plori's remote MCP server (`https://api.plori.ai/mcp`). On first
use the server asks you to sign in with your email in the browser (OAuth 2.1, one-time
code, no password).

## What you can do

- **Agents**: `list_agents`, `get_agent`, `create_agent`, `set_agent_model`,
  `delete_agent`
- **Runs**: `invoke_agent`, `get_run_result`, `cancel_run`, `list_runs`
- **Human-in-the-loop**: `list_pending_inputs`, `answer_pending_input`
- **Scheduling**: `schedule_run` for deferred work
- **Connections**: `list_connections`
- **Workflows**: `list_workflows`, `get_workflow`, `get_workflow_version`,
  `create_workflow`, `edit_workflow`, `run_workflow`,
  `list_workflow_executions`, `get_workflow_execution`
- **Account**: `get_credits`, `get_usage`, `get_disk`

## Notes

- Creating and invoking agents spends plori credits from the signed-in account;
  read-only tools are free. Pricing: https://plori.ai/pricing
- A good first prompt: "List my plori agents and show my current balance."
- More for agents: https://plori.ai/agents.md and https://plori.ai/llms.txt
