---
model: 'gpt-5.1-codex-max'
tools: ['search/codebase', 'read/readFile', 'search']
description: 'Perform code review using ChatGPT'
---
Read `.github/prompts/review/review.prompt.md` and follow its review guidelines.

Apply the problem statement, proposed solution, scope, and concern threshold provided in the user's message.
