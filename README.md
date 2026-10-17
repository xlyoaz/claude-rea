# claude-rea

Claude Code workspace with [REA (Reverse Engineer Anything)](https://github.com/morluto/rea) installed at project scope.

- `.mcp.json` registers the REA MCP server (`npx -y rea-agents@6.5.0 mcp`).
- `.claude/skills/reverse-engineer-anything/` is REA's bundled workflow skill (MIT, copied from morluto/rea v6.5.0).

Open this directory in Claude Code and approve the `rea` MCP server when prompted.
Native binary analysis additionally needs Hopper, Ghidra or IDA; JavaScript/Electron
analysis works without them. To update, bump the version in `.mcp.json` and re-copy
the skill from the matching release.
