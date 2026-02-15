---
model: 'claude-opus-4.5'
tools: ['search/codebase', 'read/readFile', 'search']
description: 'Perform code review using Claude Opus'
---
Read `.github/prompts/review/review.prompt.md` and follow its review guidelines.

Apply the problem statement, proposed solution, scope, and concern threshold provided in the user's message.
