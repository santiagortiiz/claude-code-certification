# Hooks
Execute some commands before or after claude code does something or block claude's action.
- Run code formatter
- Run tests
- Stop claude editing or reading a file
- Block file edits that does not follow naming conventions
- Check for TODO comments in code that claude writes and add them to a log file
- Block deprecated function usage

**Tip**
- for claude: list out the names of all the tools you have access to, bullet point list.
  - grep and read can read files

**Building a hook**
1. Decide on Pre/PostToolUse hook
2. Determine which type of tool call you want to watch for
3. Write a command that will receive the tool call
4. If needed, command should provide feedback to claude