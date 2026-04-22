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

## Using this skill in a workspace

Besides adding the skill folder itself, you can also add a short note in your workspace `AGENTS.md` so OpenClaw understands when and how to use the skill more consistently.

This is useful because `AGENTS.md` acts like workspace-level operating guidance. It can tell OpenClaw:
- when the skill should be used,
- what kinds of user phrasing should trigger it,
- which reference files matter in different situations,
- and how to avoid using the skill too broadly.

### Example `AGENTS.md` note

```md
- `it-role-handoff`
  - Use when the user asks the assistant to act from a specific org role such as Executive Director, IT Director, Operational Director, Information Technology Manager, QA, DBA, Web Developer, Mobile Developer, Product & Project Manager, UI/UX Designer, Graphic Designer, Product Designer, Business Analyst, or General Administration.
  - Also use when the user phrases it casually, for example: `jadi dba`, `jadi qa`, `jadi web dev`, `ambil peran business analyst`, `jawab sebagai IT Director`, or asks from a role's sudut pandang.
  - When using it, identify the intended role first, then load only the references that matter:
    - `role-synonyms.md` for abbreviations or casual phrasing
    - `role-selection-rules.md` for ambiguous role names like PM, designer, dev, admin, or director
    - `role-boundaries.md` and `anti-patterns.md` to avoid unrealistic cross-role answers
    - `handoff-patterns.md` and `multi-role-response-rules.md` when the request moves across roles
    - `output-modes.md`, `default-response-shape.md`, and `assets/templates/` when shaping the answer
  - Keep each role grounded in its own scope. Do not flatten multiple roles into one generic answer.
```

### Why this helps

Adding this kind of note to `AGENTS.md` gives OpenClaw extra workspace context about:
- how this skill fits your workflow,
- how your users are likely to invoke it,
- and what good usage looks like in practice.

The skill can still work without this note, but adding it makes the behavior more explicit and more reliable inside your own workspace.

## Notes

This repository currently reflects a practical organizational-role pattern shaped around IT, operations, product, design, QA, and administration workflows, but the structure can be adapted for broader organizational use.

## License

MIT
