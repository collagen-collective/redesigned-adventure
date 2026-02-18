# Copilot Template
This repository adds a basic setup for some helpful Copilot tools.

## `multi-review` Agent
This is a `GPT-4o-mini` agent that orchestrates code review.

It hands off user input (see `prompts/review/review.prompt.md`) to three different subagents:
- `agents/review/claude`
- `agents/review/gemini`
- `agents/review/gpt`

Each of these will perform review according to the `review.prompt.md`.

Then, `agents/review/synthesizer` will combine the review results in to a final summary.

This synthesized report will note what the agents agreed and disagreed on.

`GPT-4o-mini` is used as the orchestrator because it just needs to follow the workflow and hand off tasks. Using a lightweight model for this feels like a natural choice.
