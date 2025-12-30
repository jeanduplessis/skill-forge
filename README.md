# SkillCreator v3.0

The ultimate meta-skill for generating best-in-class Claude Code skills.

## Overview

SkillCreator v3.0 uses a 4-phase architecture to produce skills that are comprehensively analyzed, thoroughly specified, cleanly generated, and unanimously approved by a multi-agent synthesis panel.

```
┌─────────────────────────────────────────────────────────────────┐
│                    SKILLCREATOR v3.0                             │
├─────────────────────────────────────────────────────────────────┤
│ Phase 1: Deep Analysis                                           │
│   • Regression questioning loop (until exhausted)                │
│   • 11 thinking lenses applied                                   │
│   • Expert perspective simulation                                │
├─────────────────────────────────────────────────────────────────┤
│ Phase 2: Specification Generation                                │
│   • XML-structured SKILL_SPEC                                    │
│   • Explicit WHY statements                                      │
│   • Success criteria defined                                     │
├─────────────────────────────────────────────────────────────────┤
│ Phase 3: Skill Generation                                        │
│   • Fresh context execution                                      │
│   • Zero error standard                                          │
│   • Template-based output                                        │
├─────────────────────────────────────────────────────────────────┤
│ Phase 4: Multi-Agent Synthesis                                   │
│   • Design/Architecture Agent                                    │
│   • Audience/Usability Agent                                     │
│   • Evolution/Timelessness Agent                                 │
│   • Unanimous 3/3 required                                       │
└─────────────────────────────────────────────────────────────────┘
```

## Features

- **Fully Autonomous** - Provide a goal, skill iterates until best result
- **Always Maximum Depth** - Every skill gets comprehensive treatment
- **Evolution-First Design** - Skills must score ≥7/10 on timelessness
- **Multi-Lens Analysis** - 11 thinking models systematically applied
- **Regression Questioning** - Loops until 3 consecutive rounds yield no new insights
- **Multi-Agent Synthesis** - Three Opus agents must unanimously approve

## Installation

Copy to your Claude Code skills directory:

```bash
cp -r skillcreator ~/.claude/skills/
```

## Usage

Invoke with natural language:
- "create a skill for..."
- "skillcreator: build a skill that..."
- "I need a new skill for..."

Or directly:
```
Skill(skill="skillcreator")
```

## Directory Structure

```
skillcreator/
├── SKILL.md                          # Main skill definition (679 lines)
├── README.md                         # This file
├── LICENSE                           # MIT License
├── references/
│   ├── regression-questions.md       # Question bank for deep analysis
│   ├── multi-lens-framework.md       # 11 thinking model application guide
│   ├── specification-template.md     # XML spec template documentation
│   ├── evolution-scoring.md          # Timelessness scoring rubric
│   └── synthesis-protocol.md         # Multi-agent panel protocol
├── assets/
│   └── templates/
│       ├── skill-spec-template.xml   # Structured specification template
│       └── skill-md-template.md      # Output skill markdown template
└── scripts/
    └── validate-skill.py             # Python validation script
```

## The 11 Thinking Lenses

| Lens | Question |
|------|----------|
| First Principles | What are the fundamental truths here? |
| Inversion | What would make this fail? |
| Second-Order Effects | What are the downstream consequences? |
| Pre-Mortem | It's 6 months later and this failed - why? |
| Systems Thinking | How does this interact with other parts? |
| Devil's Advocate | What's the strongest argument against this? |
| Constraint Analysis | What constraints am I not seeing? |
| Pareto Analysis | What 20% will deliver 80% of value? |
| Root Cause | Why? Why? Why? Why? Why? |
| Comparative Analysis | How do similar solutions handle this? |
| Opportunity Cost | What am I NOT doing by doing this? |

## Evolution/Timelessness Scoring

All generated skills must score ≥7/10:

| Score | Classification | Lifespan |
|-------|----------------|----------|
| 1-2 | Ephemeral | Weeks |
| 3-4 | Short-lived | 6-12 months |
| 5-6 | Moderate | 1-2 years |
| 7-8 | Solid (Required) | 2-4 years |
| 9-10 | Timeless | 5+ years |

## Multi-Agent Synthesis Panel

Three Opus 4.5 agents evaluate generated skills:

| Agent | Focus | Key Criteria |
|-------|-------|--------------|
| Design/Architecture | Structure, patterns | Logical phases, no contradictions |
| Audience/Usability | Clarity, discoverability | Natural triggers, clear steps |
| Evolution/Timelessness | Future-proofing | Score ≥7, extension points |

**Unanimous 3/3 approval required.** Max 5 iteration rounds.

## Validation

Run structural validation on any skill:

```bash
python scripts/validate-skill.py /path/to/skill/
```

Validates:
- YAML frontmatter (name, version, description, license, model)
- Trigger phrases (3-5 required)
- Process/Phase sections
- Verification checkboxes
- Anti-patterns section
- Extension points

## Requirements

- Claude Code CLI
- Claude Opus 4.5 model access
- Python 3.8+ (for validation script)

## License

MIT License - see [LICENSE](LICENSE)

## Author

Created with SkillCreator v3.0 methodology.
