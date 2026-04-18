---
type: tool-profile
tool: gemini
tags:
  - planning
  - reasoning
  - architecture
use_cases:
  - planning
  - architecture
  - prompt-generation
confidence: medium
last_reviewed: 2026-04-18
---

## Strengths
- Handles very large context windows well
- Strong at high-level reasoning and planning
- Good at synthesising lots of information
- Useful for structuring problems and systems

## Weaknesses
- Less reliable for direct code execution
- Can produce vague or generic outputs
- Not as strong at precise implementation details

## Best for
- Acting as the "architect" in a multi-AI workflow
- Planning apps and systems
- Writing prompts for coding agents
- Analysing large codebases or documentation

## Avoid when
- You need precise code written correctly first time
- You are implementing complex logic directly
- Tasks require strict execution accuracy

## Prompt Formula
Goal + Context + Structure + Output Format

## Example Good Prompt
"Design the architecture for a SaaS dashboard app. Include frontend, backend, database, and auth. Output a structured plan with components and responsibilities."

## Failure Patterns
- Produces generic or surface-level plans
- Lacks implementation depth
- Overexplains instead of deciding
- Misses practical constraints

## Key Principles
- Use for thinking, not doing
- Pair with a coding agent (Claude Code / Codex)
- Force structured outputs (lists, steps, schemas)
- Always follow with execution via another model

## Role in System
Gemini = Architect  
Claude Code / Codex = Builder  

## Related
[[Planning Prompt Template]]
[[Decision Rules - Model Selection]]
[[Task Pattern - Build MVP App]]
