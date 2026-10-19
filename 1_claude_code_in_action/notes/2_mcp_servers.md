# MCP servers
- Adds new functionalities
- installed locally or remote
- playwright MCP server
  - tool to open the browser
  - tool to run code in the browser
  - tool to navigate to an address
  - tool to click on the screen

in the terminal (not claude):
claude mcp add playwright npx @playwright/mcp@latest

.claude/settings.local.json
{
    "permissions": {
        "allow": ["mcp__playwright"],
        "deny": []
    }
}

# Prompts
uigen\src\lib\prompts\generation.tsx
- assign a task and create a full component by its own and twick the prompt as needed to generate the component:

```
Your goal is to improve the component generation prompt at @src\lib\prompts\generation.tsx
Here's a real-world example of how the Playwright MCP server can improve your development workflow. Instead of manually testing and tweaking prompts, you can have Claude:

Open a browser and navigate to your application
Generate a test component
Analyze the visual styling and code quality
Update the generation prompt based on what it observes
Test the improved prompt with a new component
```