---
model: 'gemini-3-flash-preview'
tools: ['search/codebase', 'read/readFile', 'search']
description: 'Perform code review using Gemini'
---
Read `.github/prompts/review/review.prompt.md` and follow its review guidelines.

Apply the problem statement, proposed solution, scope, and concern threshold provided in the user's message.
