# FifthRow plugins

Turn business questions into structured analysis backed by original sources. The FifthRow Large Consulting Model (LCM) brings consulting agents and reusable research workflows into your chat for market sizing, competitor analysis, customer segmentation and due diligence.

Create a research App tailored to your question, or reuse a workflow whose scope matches it. Inspect its workflow and inputs, and approve its execution. Follow its progress in supported clients, explore complete reports and ask your assistant to evaluate the findings with source references.

Reuse accessible company knowledge, documents and previous research for context. Use Answers for a quick, focused public question, or set up recurring research through authorized automations.

A FifthRow account is required. Access follows your account permissions. Answers questions and results enter a shared public library; confidential information should remain in authorized company workflows.

This repository distributes plugin configuration, skills and documentation only. The hosted MCP endpoint is `https://mcp.fifthrow.com/lcm/v1`. Its backend and all credentials remain outside this repository.

## Install

The plugin folder is `plugins/fifthrow-lcm`. It includes portable OpenAI manifests, native Claude and Cursor manifests, and shared skills. Claude's marketplace is `.claude-plugin/marketplace.json`; the ChatGPT/Codex local marketplace is `.agents/plugins/marketplace.json`. Add this repository through the client's custom marketplace controls, install FifthRow: Agentic Consulting and complete OAuth. Public directory availability depends on approval and publication for each client.

Claude Code: `/plugin marketplace add fifthrow-inc/lcm`, then `/plugin install fifthrow-lcm@fifthrow`.

Codex: `codex plugin marketplace add fifthrow-inc/lcm`. Install and test through the desktop plugin directory in a new chat. Cursor: add this repository in Settings > Plugins and choose FifthRow: Agentic Consulting.

For Claude's public directory, submit the remote MCP URL as a connector and this repository's `plugins/fifthrow-lcm` folder as a plugin bundle from the same Claude organization. Pair the listings in the developer portal. Claude's custom marketplace installation alone is not a directory submission. Cursor's public marketplace takes the repository URL and reviews the plugin folder. OpenAI accepts the separately generated `openai.zip`; it does not require GitHub for this submission. Microsoft uses separately generated Microsoft 365 packages through Partner Center. Do not commit ZIPs, MCP UI bundles, backend code, account fixtures or secrets into this repository.

## Documentation and support

Read [the plugin documentation](plugins/fifthrow-lcm/README.md) for setup, account requirements, background work, lossless outputs and data boundaries. Contact support@fifthrow.com for help. Public Answers inputs and results are globally shared; confidential information belongs in authorized company workflows.

## Releases

Update the manifests' version together. Review readable skills and MCP configuration before publishing. Claude validates the tracked branch or tag and may use a GitHub push webhook. A new public listing requires its own approval; a local marketplace installation does not create one.

## License

MIT for this repository's plugin artifacts. The FifthRow hosted service and backend are separate. See LICENSE.
