# org-role-handoff

An OpenClaw skill for role-based responses, realistic scope boundaries, and structured handoffs across organizational roles.

## What this is

`org-role-handoff` is an OpenClaw skill that helps an agent respond from the perspective of a specific organizational role instead of collapsing everything into one generic voice.

It is designed for situations where the user wants the assistant to act as a role such as:
- Executive Director
- IT Director
- Operational Director
- Information Technology Manager
- Quality Assurance
- Database Administrator
- Web Developer
- Mobile Developer
- Product & Project Manager
- UI/UX Designer
- Graphic Designer
- Product Designer
- Business Analyst
- General Administration

The skill keeps each role grounded in its own:
- responsibilities
- scope
- boundaries
- collaboration context
- preferred output shape

It also supports realistic handoffs between roles, for example:
- Business Analyst → Web Developer
- UI/UX Designer → Mobile Developer
- Web Developer → QA
- IT Director → IT Manager

## Why it exists

Most assistants tend to answer multi-role organizational questions with a blended, unrealistic response.

This skill exists to make role-based responses more useful by helping the agent:
- stay inside the requested role
- avoid overclaiming authority
- handle ambiguous role names more carefully
- structure responses in a way that fits the role
- show downstream handoffs when another role should take over

## Features

- role-based perspective handling
- role synonyms and casual trigger phrasing
- ambiguous role selection rules
- role boundaries and anti-pattern guidance
- collaboration and handoff patterns
- default response shapes by role
- templates for structured outputs
- multi-role response rules

## Skill structure

```text
org-role-handoff/
├── SKILL.md
├── references/
│   ├── anti-patterns.md
│   ├── collaboration-rules.md
│   ├── default-response-shape.md
│   ├── examples.md
│   ├── handoff-patterns.md
│   ├── org-context.md
│   ├── output-modes.md
│   ├── role-boundaries.md
│   ├── role-definitions.md
│   ├── role-selection-rules.md
│   └── role-synonyms.md
├── assets/
│   └── templates/
│       ├── checklist.md
│       ├── recommendation.md
│       ├── role-brief.md
│       └── task-output.md
└── scripts/
    └── validate_role_scope.py
```

## Example prompts

- "Act as Database Administrator and review this schema."
- "Jadi QA dan bikin checklist test buat login flow ini."
- "Ambil peran Business Analyst lalu breakdown requirement fitur ini."
- "Jawab sebagai IT Director, apakah arah sistem ini masuk akal?"
- "Act as Business Analyst first, then show what the Web Developer would need next."

## Use cases

This skill is useful for:
- product and feature planning
- scoped role-based reviews
- implementation handoffs
- requirement clarification
- design-to-development transitions
- technical and organizational coordination
- multi-role response workflows

## Notes

This repository currently reflects a practical organizational-role pattern shaped around IT, operations, product, design, QA, and administration workflows, but the structure can be adapted for broader organizational use.

## License

MIT
