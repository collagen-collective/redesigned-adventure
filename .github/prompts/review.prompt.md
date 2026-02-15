---
agent: 'agent'
tools: ['search/codebase', 'vscode/askQuestions', 'read/readFile', 'search', 'todo']
description: 'Perform code review'
argument-hint: 'problemStatement, proposedSolution, inScope, outOfScope, concernThreshold:major|minor|both'
---
Problem/Task: ${input:problemStatement:What is the problem we are trying to solve? }

Proposed Solution: ${input:proposedSolution:What is the proposed solution? }

Please review the implementation against the specified problem/task and proposed solution.

Please identify any potential issues, including but not limited to:
- Potential bugs
- Oversights
- Opportunities to simplify
- Opportunities to improve readability
- Opportunities to improve maintainability
- Opportunities to make code more self-documenting

In Scope: ${input:inScope:What is in scope for this review? }
Out-of-Scope: ${input:outOfScope:What is out of scope for this review? }
Concern Threshold: ${input:concernThreshold:Should review include minor issues, major issues, or both? }
