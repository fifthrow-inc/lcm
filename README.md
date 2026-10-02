# FifthRow plugins

FifthRow provides reusable research Apps for market sizing, competitor analysis, customer segmentation and due diligence. Discover a workflow, inspect its inputs and start an authorized analysis. Read company knowledge, documents and existing reports, research narrow public questions with Answers, and manage requested recurring automations. Results include original source references and paged full outputs. Background task cards and automatic assistant continuation depend on the client. A FifthRow account is required. Public Answers questions and results enter a globally shared library; confidential information belongs only in authorized company workflows.

This repository distributes plugin configuration, skills and documentation only. The hosted MCP endpoint is `https://mcp.fifthrow.com/lcm/v1`. Its backend and all credentials remain outside this repository.

## Install

The plugin folder is `plugins/fifthrow-lcm`. It includes portable OpenAI manifests, native Claude and Cursor manifests, and shared skills. Claude's marketplace is `.claude-plugin/marketplace.json`; the ChatGPT/Codex local marketplace is `.agents/plugins/marketplace.json`. Add this repository through the client's custom marketplace controls, install FifthRow LCM and complete OAuth. Public directory availability depends on approval and publication for each client.

Claude Code: `/plugin marketplace add fifthrow-inc/lcm`, then `/plugin install fifthrow-lcm@fifthrow`.

Codex: `codex plugin marketplace add fifthrow-inc/lcm`. Install and test through the desktop plugin directory in a new chat. Cursor: add this repository in Settings > Plugins and choose FifthRow LCM.

Directory submissions point Claude and Cursor at `plugins/fifthrow-lcm`. OpenAI accepts the separately generated `openai.zip`; it does not require GitHub for this submission. Microsoft uses separately generated Microsoft 365 packages through Partner Center. Do not commit ZIPs, MCP UI bundles, backend code, account fixtures or secrets into this repository.

## Documentation and support

Read [the plugin documentation](plugins/fifthrow-lcm/README.md) for setup, account requirements, background work, lossless outputs and data boundaries. Contact support@fifthrow.com for help. Public Answers inputs and results are globally shared; confidential information belongs in authorized company workflows.

## Releases

Update the manifests' version together. Review readable skills and MCP configuration before publishing. Claude validates the tracked branch or tag and may use a GitHub push webhook. A new public listing requires its own approval; a local marketplace installation does not create one.

## License

MIT for this repository's plugin artifacts. The FifthRow hosted service and backend are separate. See LICENSE.
