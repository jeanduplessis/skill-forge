---
name: skillcreator
version: 3.0.0
description: >
  Ultimate meta-skill for creating production-ready Claude Code skills. Uses deep
  iterative analysis with 11 thinking models, regression questioning until exhausted,
  evolution/timelessness as core lens, and multi-agent synthesis panel for unanimous
  approval. Fully autonomous execution at maximum depth produces categorically the
  best possible skills.
license: MIT
model: claude-opus-4-5-20251101
subagent_model: claude-opus-4-5-20251101
domains: [meta-skill, automation, skill-creation, orchestration]
type: orchestrator
inputs: [user-goal, domain-hints]
outputs: [SKILL.md, references/, SKILL_SPEC.md]
---

# SkillCreator 3.0 - Ultimate Meta-Skill

Create categorically the best possible Claude Code skills through exhaustive analysis,
multi-lens evaluation, and multi-agent synthesis.

**Philosophy:** A skill that the audience would unanimously agree is the very best
possible result they could have received.

## Triggers

- \`SkillCreator: {goal}\` - Full autonomous skill creation
- \`create skill\` / \`new skill\` - Natural language activation
- \`design skill for {purpose}\` - Purpose-first creation
- \`ultimate skill\` - Emphasize maximum quality
- \`skillcreator --plan-only\` - Generate specification without execution

## Quick Reference

| Input | Output | Duration | Quality Gate |
|-------|--------|----------|--------------|
| User goal | Production skill | 5-15 min | Unanimous 3/3 panel |
| Domain hints (optional) | SKILL.md + references | Variable | Timelessness ≥7 |

## Architecture Overview

\`\`\`
┌─────────────────────────────────────────────────────────────────────────┐
│                       SKILLCREATOR 3.0                                   │
│                    Ultimate Meta-Skill                                   │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                          │
│  PHASE 1: DEEP ANALYSIS ──────────────────────────────────────────────  │
│  │ Single Opus Agent • Iterative • Until Exhausted                      │
│  │                                                                       │
│  │  ┌──────────────┐   ┌────────────────┐   ┌─────────────────┐         │
│  │  │ 1A: INPUT    │──▶│ 1B: MULTI-LENS │──▶│ 1C: REGRESSION  │──┐      │
│  │  │ EXPANSION    │   │ ANALYSIS       │   │ QUESTIONING     │  │      │
│  │  └──────────────┘   └────────────────┘   └─────────────────┘  │      │
│  │        ▲                                                       │      │
│  │        └───────────────────────────────────────────────────────┘      │
│  │                    Loop until 3 empty rounds                          │
│  │                                                                       │
├──┼───────────────────────────────────────────────────────────────────────┤
│                                                                          │
│  PHASE 2: SPECIFICATION GENERATION ────────────────────────────────────  │
│  │ Meta-prompting pattern • XML-structured                               │
│  │                                                                       │
│  │  Analysis insights → Rigorous SKILL_SPEC.md                          │
│  │  • Explicit WHY for all decisions                                    │
│  │  • Measurable success criteria                                       │
│  │  • Evolution/timelessness analysis                                   │
│  │                                                                       │
├──┼───────────────────────────────────────────────────────────────────────┤
│                                                                          │
│  PHASE 3: SKILL GENERATION ────────────────────────────────────────────  │
│  │ Fresh context • Zero error standard                                   │
│  │                                                                       │
│  │  Execute SKILL_SPEC.md with clean context                            │
│  │  • Write SKILL.md                                                    │
│  │  • Generate references/                                              │
│  │  • Create assets/ if needed                                          │
│  │                                                                       │
├──┼───────────────────────────────────────────────────────────────────────┤
│                                                                          │
│  PHASE 4: MULTI-AGENT SYNTHESIS ───────────────────────────────────────  │
│  │ 3 Opus Agents • Parallel • Unanimous Required                         │
│  │                                                                       │
│  │  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐                   │
│  │  │ DESIGN      │  │ AUDIENCE    │  │ EVOLUTION   │                   │
│  │  │ Architecture│  │ Usability   │  │ Timelessness│                   │
│  │  │ Correctness │  │ Clarity     │  │ Extensibility│                  │
│  │  └─────────────┘  └─────────────┘  └─────────────┘                   │
│  │         │               │               │                             │
│  │         └───────────────┼───────────────┘                             │
│  │                         ▼                                             │
│  │                 ┌───────────────┐                                     │
│  │                 │ UNANIMOUS 3/3 │                                     │
│  │                 └───────────────┘                                     │
│  │                    │         │                                        │
│  │              Yes ──┘         └── No → Return to Phase 1               │
│  │                │                                                      │
│  │                ▼                                                      │
│  │         ┌────────────┐                                                │
│  │         │ FINALIZE   │                                                │
│  │         └────────────┘                                                │
│                                                                          │
└─────────────────────────────────────────────────────────────────────────┘
\`\`\`

---

## Phase 1: Deep Analysis

**Agent:** Single Opus 4.5 with extended thinking
**Duration:** 3-7 analysis cycles
**Goal:** Exhaust all analytical perspectives before designing

### 1A: Input Expansion

Transform user's goal into comprehensive requirements:

\`\`\`
USER INPUT: "Create a skill for X"
                │
                ▼
┌─────────────────────────────────────────────────────────────┐
│ EXPLICIT REQUIREMENTS                                        │
│ • What the user literally asked for                          │
│ • Direct functionality stated                                │
├─────────────────────────────────────────────────────────────┤
│ IMPLICIT REQUIREMENTS                                        │
│ • What they probably expect but didn't say                   │
│ • Standard quality expectations                              │
│ • Integration with existing patterns                         │
├─────────────────────────────────────────────────────────────┤
│ UNKNOWN UNKNOWNS                                             │
│ • What they don't know they need                             │
│ • Expert-level considerations they'd miss                    │
│ • Future needs they haven't anticipated                      │
├─────────────────────────────────────────────────────────────┤
│ DOMAIN CONTEXT                                               │
│ • Related skills that exist                                  │
│ • Patterns from similar skills                               │
│ • Lessons from skill failures                                │
└─────────────────────────────────────────────────────────────┘
\`\`\`

**Check for overlap with existing skills:**
\`\`\`bash
ls ~/.claude/skills/
# Grep for similar triggers in existing SKILL.md files
\`\`\`

| Match Score | Action |
|-------------|--------|
| >7/10 | Use existing skill instead |
| 5-7/10 | Clarify distinction before proceeding |
| <5/10 | Proceed with new skill |

### 1B: Multi-Lens Analysis

Apply all 11 thinking models systematically:

| Lens | Core Question | Application |
|------|---------------|-------------|
| **First Principles** | What's fundamentally needed? | Strip convention, find core |
| **Inversion** | What guarantees failure? | Build anti-patterns |
| **Second-Order** | What happens after the obvious? | Map downstream effects |
| **Pre-Mortem** | Why did this fail? | Proactive risk mitigation |
| **Systems Thinking** | How do parts interact? | Integration mapping |
| **Devil's Advocate** | Strongest counter-argument? | Challenge every decision |
| **Constraints** | What's truly fixed? | Separate real from assumed |
| **Pareto** | Which 20% delivers 80%? | Focus on high-value features |
| **Root Cause** | Why is this needed? (5 Whys) | Address cause not symptom |
| **Comparative** | How do options compare? | Weighted decision matrix |
| **Opportunity Cost** | What are we giving up? | Explicit trade-offs |

**Minimum requirement:** All 11 lenses scanned, at least 5 applied in depth.

See: [references/multi-lens-framework.md](references/multi-lens-framework.md)

### 1C: Regression Questioning

Iterative self-questioning until no new insights emerge:

\`\`\`
ROUND N:
│
├── "What am I missing?"
├── "What would an expert in {domain} add?"
├── "What would make this fail?"
├── "What will this look like in 2 years?"
├── "What's the weakest part of this design?"
└── "Which thinking model haven't I applied?"
    │
    └── New insights > 0?
        │
        ├── YES → Incorporate and loop
        └── NO → Check termination criteria
\`\`\`

**Termination Criteria:**
- Three consecutive rounds produce no new insights
- All 11 thinking models have been applied
- At least 3 simulated expert perspectives considered
- Evolution/timelessness explicitly evaluated

**Red Flags (restart questioning):**
- Uncertainty language ("might", "possibly", "I think")
- Missing justification for decisions
- Timelessness score < 7

See: [references/regression-questions.md](references/regression-questions.md)

---

## Phase 2: Specification Generation

**Pattern:** Meta-prompting (separate analysis from execution)
**Goal:** Produce rigorous specification that enables clean Phase 3 execution

### Specification Structure

The specification captures all analysis insights in XML format:

\`\`\`xml
<skill_specification>
  <metadata>
    <name>skill-name</name>
    <analysis_iterations>N</analysis_iterations>
    <timelessness_score>X/10</timelessness_score>
  </metadata>

  <context>
    <problem_statement>What + Why + Who</problem_statement>
    <existing_landscape>Related skills, distinctiveness</existing_landscape>
  </context>

  <requirements>
    <explicit>What user asked for</explicit>
    <implicit>Expected but unstated</implicit>
    <discovered>Found through analysis</discovered>
  </requirements>

  <architecture>
    <pattern>Selected pattern with WHY</pattern>
    <phases>Ordered phases with verification</phases>
    <decision_points>Branches and defaults</decision_points>
  </architecture>

  <evolution_analysis>
    <timelessness_score>X/10</timelessness_score>
    <extension_points>Where skill can grow</extension_points>
    <obsolescence_triggers>What would break it</obsolescence_triggers>
  </evolution_analysis>

  <anti_patterns>
    <pattern>What to avoid + WHY + alternative</pattern>
  </anti_patterns>

  <success_criteria>
    <criterion>Measurable + verification method</criterion>
  </success_criteria>
</skill_specification>
\`\`\`

See: [references/specification-template.md](references/specification-template.md)

### Specification Validation

Before proceeding to Phase 3:

- [ ] All sections present with no placeholders
- [ ] Every decision includes WHY
- [ ] Timelessness score ≥ 7 with justification
- [ ] At least 2 extension points documented
- [ ] All requirements traceable to source

---

## Phase 3: Skill Generation

**Context:** Fresh, clean (no analysis artifacts polluting)
**Standard:** Zero errors—every section verified before proceeding

### Generation Order

\`\`\`
1. Create directory structure
   mkdir -p ~/.claude/skills/{skill-name}/references
   mkdir -p ~/.claude/skills/{skill-name}/assets/templates

2. Write SKILL.md
   • Frontmatter (YAML)
   • Title and brief intro
   • Triggers (3-5 varied phrases)
   • Quick Reference table
   • Process (phases/steps)
   • Anti-Patterns
   • Verification criteria
   • Evolution/Extension Points
   • References

3. Generate reference documents (if needed)
   • Deep documentation for complex topics
   • Templates for generated artifacts
   • Checklists for validation

4. Create assets (if needed)
   • Templates for skill outputs
   • Validation scripts
\`\`\`

### Quality Checks During Generation

| Check | Requirement |
|-------|-------------|
| Frontmatter | name, version, description, license, model |
| Triggers | 3-5 distinct, natural language |
| Phases | 1-3 max, not over-engineered |
| Verification | Concrete, measurable |
| Tables over prose | Structured information in tables |
| No placeholder text | Every section fully written |

---

## Phase 4: Multi-Agent Synthesis

**Panel:** 3 Opus agents with distinct evaluative lenses
**Requirement:** Unanimous 3/3 approval
**Fallback:** Return to Phase 1 with feedback (max 5 iterations)

### Panel Composition

| Agent | Focus | Key Criteria |
|-------|-------|--------------|
| **Design/Architecture** | Structure, patterns, correctness | Pattern appropriate, phases logical, no circular deps |
| **Audience/Usability** | Clarity, discoverability, completeness | Triggers natural, steps unambiguous, no assumed knowledge |
| **Evolution/Timelessness** | Future-proofing, extension, ecosystem | Score ≥7, extension points clear, ecosystem fit |

### Agent Evaluation

Each agent produces:

\`\`\`markdown
## [Agent] Review

### Verdict: APPROVED / CHANGES_REQUIRED

### Scores
| Criterion | Score (1-10) | Notes |
|-----------|--------------|-------|

### Strengths
1. [Specific with evidence]

### Issues (if CHANGES_REQUIRED)
| Issue | Severity | Required Change |
|-------|----------|-----------------|

### Recommendations
1. [Even if approved]
\`\`\`

### Consensus Protocol

\`\`\`
IF all 3 agents APPROVED:
    → Finalize skill
    → Update registry
    → Complete

ELSE:
    → Collect all issues
    → Return to Phase 1 with issues as input
    → Re-apply targeted questioning
    → Regenerate skill
    → Re-submit to panel

IF 5 iterations without consensus:
    → Flag for human review
    → Present all agent perspectives
    → User makes final decision
\`\`\`

See: [references/synthesis-protocol.md](references/synthesis-protocol.md)

---

## Evolution/Timelessness Core Lens

Every skill is evaluated through the evolution lens:

### Temporal Projection

| Timeframe | Key Question |
|-----------|--------------|
| 6 months | How will usage patterns evolve? |
| 1 year | What ecosystem changes are likely? |
| 2 years | What new capabilities might obsolete this? |
| 5 years | Is the core problem still relevant? |

### Timelessness Scoring

| Score | Description | Verdict |
|-------|-------------|---------|
| 1-3 | Transient, will be obsolete in months | Reject |
| 4-6 | Moderate, depends on current tooling | Revise |
| **7-8** | **Solid, principle-based, extensible** | **Approve** |
| 9-10 | Timeless, addresses fundamental problem | Exemplary |

**Requirement:** All skills must score ≥7.

### Anti-Obsolescence Patterns

| Do | Don't |
|----|-------|
| Design around principles | Hardcode implementations |
| Document the WHY | Only document the WHAT |
| Include extension points | Create closed systems |
| Abstract volatile dependencies | Direct coupling |
| Version-agnostic patterns | Pin specific versions |

See: [references/evolution-scoring.md](references/evolution-scoring.md)

---

## Architecture Pattern Selection

Select based on task complexity:

| Pattern | Use When | Structure |
|---------|----------|-----------|
| **Single-Phase** | Simple linear tasks | Steps 1-2-3 |
| **Checklist** | Quality/compliance audits | ☐ Item verification |
| **Generator** | Creating artifacts | Input → Transform → Output |
| **Multi-Phase** | Complex ordered workflows | Phase 1 → Phase 2 → Phase 3 |
| **Multi-Agent Parallel** | Independent subtasks | Launch agents concurrently |
| **Multi-Agent Sequential** | Dependent subtasks | Agent 1 → Agent 2 → Agent 3 |
| **Orchestrator** | Coordinating multiple skills | Meta-skill chains |

### Selection Decision Tree

\`\`\`
Is it a simple procedure?
├── Yes → Single-Phase
└── No → Does it produce artifacts?
    ├── Yes → Generator
    └── No → Does it verify/audit?
        ├── Yes → Checklist
        └── No → Are subtasks independent?
            ├── Yes → Multi-Agent Parallel
            └── No → Multi-Agent Sequential or Multi-Phase
\`\`\`

---

## Skill Directory Structure

\`\`\`
~/.claude/skills/{skill-name}/
├── SKILL.md                    # Main entry point (required)
├── references/                 # Deep documentation (optional)
│   ├── patterns.md
│   ├── examples.md
│   └── configuration.md
├── assets/                     # Templates, checklists (optional)
│   └── templates/
└── scripts/                    # Validation tools (optional)
\`\`\`

---

## Required SKILL.md Elements

| Element | Purpose | Requirement |
|---------|---------|-------------|
| Frontmatter | Metadata | name, version, description, license, model |
| Title | Skill name | H1 with descriptive title |
| Triggers | Activation phrases | 3-5 distinct, natural language |
| Quick Reference | Summary table | Input, output, key info |
| Process | Execution steps | Numbered phases or tables |
| Anti-Patterns | What to avoid | With WHY and alternative |
| Verification | Success criteria | Concrete, measurable |
| Evolution | Extension points | At least 2 documented |

### Frontmatter Template

\`\`\`yaml
---
name: skill-name
version: 1.0.0
description: >
  One-paragraph description of what this skill does, when to use it,
  and what it produces. Be specific about inputs and outputs.
license: MIT
model: claude-opus-4-5-20251101
---
\`\`\`

---

## Anti-Patterns

| Avoid | Why | Instead |
|-------|-----|---------|
| Creating duplicate skills | Bloats registry, confuses | Check existing first |
| Single trigger phrase | Hard to discover | Use 3-5 varied phrases |
| No verification criteria | Can't confirm success | Define measurable outcomes |
| Over-engineering | Complexity without value | Start simple, iterate |
| Vague descriptions | Doesn't help selection | Be specific about purpose |
| Prose walls | Hard to scan | Use tables and lists |
| Missing WHY | Can't evolve or maintain | Document rationale |
| Hardcoded dependencies | Obsolescence risk | Abstract and configure |
| No extension points | Can't grow | Design for evolution |
| Premature termination | Suboptimal result | Question until exhausted |

---

## Verification Checklist

After skill creation:

### Structural
- [ ] SKILL.md has valid frontmatter
- [ ] 3-5 trigger phrases defined
- [ ] Process/phases documented
- [ ] Verification criteria included
- [ ] Anti-patterns section present

### Content
- [ ] No placeholder text
- [ ] All decisions include WHY
- [ ] Examples where helpful
- [ ] No unexplained jargon

### Evolution
- [ ] Timelessness score ≥ 7
- [ ] At least 2 extension points
- [ ] Dependencies abstracted
- [ ] Composes with ecosystem

### Registration
- [ ] Added to \`registry.md\`
- [ ] Updated \`CAPABILITIES.md\`
- [ ] Updated skill count in \`CLAUDE.md\`

---

## Commands

| Command | Action |
|---------|--------|
| \`SkillCreator: {goal}\` | Full autonomous execution |
| \`SkillCreator --plan-only {goal}\` | Generate specification only |
| \`SkillCreator --iteration N\` | Resume from iteration N |
| \`SkillCreator --quick {goal}\` | Reduced depth (not recommended) |

---

## Configuration

\`\`\`yaml
SKILLCREATOR_CONFIG:
  mode: autonomous
  depth: maximum  # always
  core_lens: evolution_timelessness

  analysis:
    min_lens_depth: 5
    max_questioning_rounds: 7
    termination_empty_rounds: 3

  synthesis:
    panel_size: 3
    require_unanimous: true
    max_iterations: 5
    escalate_to_human: true

  evolution:
    min_timelessness_score: 7
    min_extension_points: 2
    require_temporal_projection: true

  model:
    primary: claude-opus-4-5-20251101
    subagents: claude-opus-4-5-20251101
\`\`\`

---

## Examples

### Example 1: Simple Skill Request

**Input:** "Create a skill to check TypeScript types"

**Phase 1 Output (partial):**
- First Principles: Core need is catching type errors before runtime
- Inversion: Would fail if: slow, false positives, unclear output
- Systems: Integrates with verification-runner, pre-commit hooks
- Evolution: TypeScript evolving but type-checking fundamental (score: 8)

**Phase 4 Result:**
- Design Agent: APPROVED (patterns sound, phases logical)
- Audience Agent: APPROVED (triggers natural, steps clear)
- Evolution Agent: APPROVED (score 8, extensible to new TS features)
- **Consensus: 3/3 APPROVED**

### Example 2: Complex Skill Request

**Input:** "Create a skill for automated code review"

**Phase 1 Output (partial):**
- First Principles: Need unbiased, consistent code quality feedback
- Inversion: Fails if: noisy, misses real issues, too slow, not actionable
- Systems: Must compose with codereview, testgen, verification-runner
- Pareto: 80% value from: bugs, security, performance (not style nits)
- Evolution: Code review is timeless; patterns evolve (score: 7)

**Phase 4 Iteration 1:**
- Design Agent: CHANGES_REQUIRED (phase 2 lacks verification)
- Audience Agent: APPROVED
- Evolution Agent: APPROVED
- **Consensus: 2/3 → Iterate**

**Phase 4 Iteration 2:**
- All agents: APPROVED
- **Consensus: 3/3 APPROVED**

---

## References

- [Regression Questions](references/regression-questions.md) - Complete question bank
- [Multi-Lens Framework](references/multi-lens-framework.md) - 11 thinking models guide
- [Specification Template](references/specification-template.md) - XML spec structure
- [Evolution Scoring](references/evolution-scoring.md) - Timelessness evaluation
- [Synthesis Protocol](references/synthesis-protocol.md) - Multi-agent panel details

---

## Related Skills

| Skill | Relationship |
|-------|--------------|
| skill-composer | Can orchestrate created skills |
| claude-authoring-guide | Deeper patterns reference |
| codereview | Pattern for multi-agent panels |
| maker-framework | Zero error standard source |

---

## Extension Points

1. **Additional Lenses:** Add new thinking models to \`references/multi-lens-framework.md\`
2. **New Synthesis Agents:** Extend panel beyond 3 agents for specific domains
3. **Custom Patterns:** Add architecture patterns to selection guide
4. **Domain Templates:** Add domain-specific templates to \`assets/templates/\`

---

## Changelog

### v3.0.0 (Current)
- Complete redesign as ultimate meta-skill
- Added regression questioning loop
- Added multi-lens analysis framework (11 models)
- Added evolution/timelessness core lens
- Added multi-agent synthesis panel
- Fully autonomous execution
- Maximum depth always

### v2.0.0 (Previous)
- Pattern selection guide
- Quality standards checklist
- Match scoring for duplicates

### v1.0.0 (Original)
- Basic skill structure
- Directory layout
