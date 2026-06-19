1. Tools Installed
- Cursor IDE
- Node.js (v24.17.0)
- Claude Code CLI (@anthropic-ai/claude-code)
- OpenAI Codex (Built-in model configuration)

### 2. Steps Completed
- Installed and set up Cursor IDE as the primary code editor.
- Installed Node.js to enable the required package manager environment.
- Configured Windows terminal settings to correctly recognize software commands.
- Adjusted local Windows safety execution settings to allow package downloads.
- Successfully downloaded and installed the Claude Code developer agent tool via the terminal.
- Enabled OpenAI's Codex model suite natively within Cursor's internal system preferences panel.

### 3. Issues Encountered & Solutions
- *Issue 1: Codex missing from the extension marketplace search*
  - Solution: Found that Codex is natively built into the editor in newer versions. Activated it directly through Cursor Settings > Models instead of using a plugin.
- *Issue 2: Terminal stated "node-v is not recognized as an internal or external command"*
  - Solution: Fixed Windows path configuration directly inside the integrated panel by running $env:Path += ";C:\Program Files\nodejs" to link the software folder.
- *Issue 3: Windows script blocking error (Execution Policy Restriction)*
  - Solution: Temporarily bypassed the security lock for the installation process by typing Set-ExecutionPolicy Bypass -Scope Process into the command line.
