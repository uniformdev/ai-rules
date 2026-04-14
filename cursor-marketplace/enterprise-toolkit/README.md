# Enterprise Toolkit

Cursor plugin with security standards, compliance checks, and automation for enterprise development.

## Contents

- **Rules**: `security-standards.mdc`, `code-style.mdc`
- **Skills**: `compliance-check`, `security-review`
- **Agents**: `security-reviewer`, `compliance-checker`
- **Commands**: `run-compliance-scan`
- **Hooks**: afterFileEdit (format), beforeShellExecution (validate), sessionEnd (audit)
- **MCP**: Optional filesystem server (configure path in `.mcp.json`)

## Configuration

- Edit `hooks/hooks.json` to enable or disable hooks and matchers.
- Edit `.mcp.json` to add or change MCP servers (e.g. database, APIs).
- Replace placeholder scripts in `scripts/` with your formatters and validators.

## Usage

Install this plugin via the Cursor marketplace or from this repo. Rules and skills apply when the plugin is active. Use agents and commands from the Cursor UI as needed.
