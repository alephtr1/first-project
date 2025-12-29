# Council Project Instructions

## OpenRouter API
When a relevant topic comes up (API calls, model features, response formats, plugins, reasoning, streaming, etc.), check the OpenRouter documentation:

- **Main docs**: https://openrouter.ai/docs
- Navigate from there to find specific topics

Key sections:
- API Reference: parameters, chat completions, streaming
- Reasoning Tokens: for thinking models like DeepSeek R1
- Plugins: web search, PDF processing
- Model variants: :free, :thinking, :online, etc.

## Git Workflow
1. Always fetch origin/main before creating a new branch
2. Branch names must end with the session ID suffix (e.g., `-tt6dC`)
3. Push with `git push -u origin <branch-name>`
4. **Before creating a PR or when PR has conflicts**: Always rebase on latest main
   ```bash
   git fetch origin main
   git rebase origin/main
   git push --force-with-lease
   ```
5. If working on a task that might already have changes in main, fetch and check first
