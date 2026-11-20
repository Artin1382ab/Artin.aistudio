---
name: mobile-first-layout
description: "Build mobile-first user journeys and touch-friendly UI Use for related Gemini UI/UX, web development, debugging, maintenance, or coding tasks."
---

# Mobile First Layout

## When to use
Use when the user requests build mobile-first user journeys and touch-friendly ui. Select this skill only when it directly matches the active task; avoid loading unrelated skills.

## Inputs and baseline
- Identify the repository, runtime, framework and exact versions from available files rather than assuming.
- Obtain the brief, expected behavior, audience, design references, screenshots, pages, mobile breakpoints and deployment environment where relevant.
- Record immutable constraints: routes/URLs, logos, labels, brand colors, API contracts, user data and existing business rules.
- If tools/repository are inaccessible, produce a proposed implementation and clear commands without claiming that changes or tests ran.

## Specialist procedure
1. Identify core mobile task and simplify first screen.
2. Start with constrained viewport and progressively enhance.
3. Ensure tap targets, sticky bars and keyboard-safe forms.
4. Optimize imagery, loading and navigation on slow networks.
5. Validate orientation and reduced motion.

## Tool candidates
CSS, browser emulation, touch QA. Tools are suggestions only: check whether each tool, plugin, executable, authorized connection and version exists before attempting operations. Never claim to have installed or invoked unavailable tools.

## Verification and acceptance
- Touch controls usable.
- No content clipping.
- Fast critical path.
- Validate the requested runtime with actual build, lint, typecheck, tests, browser rendering, mobile checks and production-like behavior where available.
- Make the smallest safe changes, protect working code and keep reversible diffs. Do not delete unrelated files or overwrite originals without permission.
- Include the precise files changed, test commands and real results. Label any untested steps or hypothetical output clearly.

## Delivery
Provide a concise result summary, implementation decisions, artifact/file paths (when verified), test evidence, known limitations, and next actions. For visual tasks include responsive screenshots or an explicit screenshot plan; for code tasks include concrete reproduction and verification commands.

## Google AI Studio agent runtime addendum (20 November 2026)
- In Google AI Studio Agents Playground / managed agents, this skill is available only when its SKILL.md (and any referenced assets) is mounted into the agent environment under `.agents/skills/`. The model should select it only for matching tasks.
- In Google AI Studio Build mode, this document is *project reference material*; importing it does not register an account-level Skill or guarantee automatic loading. Ask the Build agent to inspect `AGENTS.md` and load relevant files as needed.
- Verify actual tool availability, network permission, file access and execution success. Do not claim a render, test, deployment, browser action, SDK installation, or access to Windows software without observed evidence.
- Never delete existing source files or overwrite project assets without explicit approval; preserve logos, brand details and contracts.
