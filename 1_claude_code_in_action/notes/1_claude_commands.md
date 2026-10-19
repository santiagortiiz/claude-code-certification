# Commands
- claude: invoke the CLI
- **/init:** analyze code base and generates CLAUDE.md
- **Commit:** Stage and commit changes
- Esc can be used to interrupt claude and provide context "# context" to redirect the conversation
- Esc + Esc: revert to a previous message and removes context not relevant to the current task
- **/compact:** Take all messages in current conversation and summarize that learning for further tasks
- **/clear:** dump the entire conversation history to start a different task

# Create custom commands
.claude/commands/new_file.md
**example**
```
audit.md
Your goal is to update any vulnerable dependencies.

Do the following:
1. Run `npm audit` to find vulnerable packages
2. Run `npm audit fix` to apply updates
3. Run tests and verify updates did not break anything.
```
**Arguments** can be passed by natural language, i.e: /write_tests the use-auth.ts file in the hooks directory

# CLAUDE.md
- Will be included on any request
- Serves as location to provide guidance
  - CLAUDE.md -> shared in the code repository
  - CLAUDE.local.md -> local
  - ~/.claude/CLAUDE.md -> all projects
- can be modified manually or in the terminal use a "#" to put claude in memory mode
  - "# Use comments sparingly. Only comment complex code."

# Planning mode
SHIFT+TAB && SHIFT+TAB (Twice)

# Thinking modes
- Think
- Think more
- Think a lot
- Think longer
- Ultrathink
**example:** This is a tough task, so ultrathink about the best way to implement it.

# Ask and reference files
How does the auth system work?
@src/components/auth/AuthDialog.tsx
@src/hooks/use.auth.ts

# Screenshoots
- Windows: Win + Shift + S && Ctrl + V is supported in the chat

