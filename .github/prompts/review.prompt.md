---
agent: 'agent'
tools: ['search/codebase', 'vscode/askQuestions', 'read/readFile', 'search', 'todo']
description: 'Perform code review'
---
Problem/Task: ${input:problemStatement:What is the problem we are trying to solve? }
Proposed Solution: ${input:proposedSolution:What is the proposed solution? }

Please review the proposed solution and identify any potential issues, including but not limited to:
- Potential bugs
- Oversights
- Opportunities to simplify
- Opportunities to improve readability
- Opportunities to improve maintainability
- Opportunities to make code more self-documenting
