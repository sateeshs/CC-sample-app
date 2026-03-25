```CC Prompt
Create a new Next.js project.
- Project name: my-app
- Follow the tech stack defined in CLAUDE.md
- Run create-next-app and complete initialization through shadcn/ui setup
```

[workflow](https://32blog.com/en/claude-code/claude-code-nextjs-app-router-mistakes-workflow)
[Next.js DevTools MCP](https://github.com/vercel/next-devtools-mcp)

`npx add-mcp next-devtools-mcp@latest`

[Templates](https://github.com/davila7/claude-code-templates/blob/main/CLAUDE.md)
```
# Single component
npx claude-code-templates@latest --agent frontend-developer
npx claude-code-templates@latest --command setup-testing
npx claude-code-templates@latest --hook automation/simple-notifications

# Batch installation
npx claude-code-templates@latest --agent security-auditor --command security-audit --setting read-only-mode

# Interactive mode
npx claude-code-templates@latest
```


[CC dashboard](http://localhost:3333/#dashboard)

[NextJs16-new-7-mistecks](https://32blog.com/en/claude-code/claude-code-nextjs-app-router-mistakes-workflow)


#### Pattern 4: Hierarchical for large projects

```
root/CLAUDE.md              # Project-wide rules (keep minimal)
src/api/CLAUDE.md           # API layer rules
src/components/CLAUDE.md    # UI layer rules
src/lib/CLAUDE.md           # Utility layer rules

```

##### How Claude remembers your project

- [Memory](https://code.claude.com/docs/en/memory)
- [workflow-2](https://github.com/CloudAI-X/claude-workflow-v2)
- [BestPractises](https://github.com/shanraisshan/claude-code-best-practice/)

##### Agent Flow:

##### Sub Agents
##### Agent Teams