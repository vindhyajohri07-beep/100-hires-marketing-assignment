1. Tools Installed
-Cursor IDE
-OpenAI Codex Integration
-Node.js (v24.17.0 LTS)
-Anthropic Claude Code CLI (@anthropic-ai/claude-code)
-Git Bash/Desktop Engine

2. Steps Completed
- Initial Setup & Authentication
Visited the official website at cursor.com and downloaded the standard Windows installation binaries.
Opened the newly installed IDE and logged in directly using my GitHub credentials (vindhyajohri07-beep), successfully linking my developer profile to the workspace.
- Cleaning & Reinstalling the IDE
Uninstalled the previous broken build of Cursor using standard Windows uninstallation protocols.
Manually deleted residual configuration and cache folders from %appdata%\Cursor and %userprofile%\.cursor.
Downloaded the latest stable .exe installer directly from cursor.com and ran it to get a clean editor environment.
- Setting Up the AI Engines
Bypassed the empty extensions marketplace and opened the master system settings via the Gear Icon (⚙️) (or Ctrl + Shift + J).
Headed to the internal Models panel, located the core GPT/Codex toggles, and switched them to Active.
Opened the chat sidebar with Ctrl + L and verified that the model dropdown menu correctly targeted the active OpenAI processing pool.
- Installing Node.js & Claude Code
Downloaded the stable prebuilt installer package from nodejs.org and installed it to C:\Program Files\nodejs\.
Opened the built-in Cursor terminal (Ctrl + \``) and ran npm install -g @anthropic-ai/claude-code`.
Ran the command claude in the console and followed the generated login link to authenticate the Anthropic environment.
-GitHub Integration & Environment Sync
Logged into GitHub via the browser and created a new public repository named 100-hires-marketing-assignment with an initialized README.md file.
Installed Git from git-scm.com so Cursor could translate version control commands, then restarted Cursor to update environment maps.
Ran git clone <repository-url> in the terminal to pull the repo down locally, then loaded it into the editor via File > Open Folder.
- Documenting & Committing the Project
Switched the workspace view back to the standard file explorer using Ctrl + Shift + E, clicked the New File icon, and named it README.md.
Pasted this deployment log into the editor workspace and saved the file using Ctrl + S.
Opened the Source Control sidebar (Ctrl + Shift + G), typed the commit message Final project report commit, clicked Commit, and hit Sync Changes to push the code live to GitHub.

3. Issues Faced & Solutions
Issue: Searching for "Codex" in the Extensions marketplace (Ctrl + Shift + X) returned zero results.
Root Cause: The external plugin is deprecated because modern builds of Cursor have Codex and OpenAI models built directly into the editor's base settings.
Solution: Abandoned the marketplace search. Clicked the Gear Icon (⚙️) to open settings, navigated to the Models tab, and turned on the model toggles manually.

Issue: The terminal threw an error stating that node -v was an unrecognized command.
Root Cause: The Node.js installer didn't automatically refresh or add its binary folder to the active Windows environment paths.
Solution: Manually patched the active terminal's path by running the command:
$env:Path += ";C:\Program Files\nodejs"

Issue: The Anthropic CLI installation failed with a Windows Scripting Lockout Error.
Root Cause: Windows background execution policies blocked the remote scripts from downloading and installing the packages globally.
Solution: Temporarily dropped the operating system restriction for the active terminal session by running:
Set-ExecutionPolicy Bypass -Scope Process

Issue: Running the git clone command returned an "unrecognized command" error.
Root Cause: The core Git version control software wasn't installed on the local machine yet.
Solution: Downloaded the Git installer from git-scm.com, completed the standard installation wizard, and restarted Cursor to refresh the terminal tracking.

Issue: Clicking the + icons kept starting new AI conversation threads instead of creating actual text files.
Root Cause: The Cursor interface layout was stuck in the full-screen AI Composer/Agent dashboard view.
Solution: Pressed Ctrl + Shift + E to force the window back into the standard File Explorer view, then used the correct New File (📄+) button.
