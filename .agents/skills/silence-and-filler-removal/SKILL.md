---
name: silence-and-filler-removal
description: Find silence and verbal filler for talking-head edits without removing meaning Use when the user asks for this capability in a video production, editing, social ad, or delivery task.
---
# Silence And Filler Removal

## Scope and activation
Find silence and verbal filler for talking-head edits without removing meaning. Applicable to planning-only Gemini Apps Tasks and to executable Gemini CLI workflows. Always distinguish planned actions from verified tool execution.

## Required inputs
Ask for or infer where unambiguous: source media or filenames, edit brief, target audience, duration, canvas aspect ratio, platform, language, brand reference, music/voiceover rights, and available tools. For missing source footage, propose a shot plan instead of pretending video exists.

## Expert procedure
1. **Step 1:** Run VAD or silence detection on a separate audio track.
2. **Step 2:** Check pause intervals against punctuation and emphasis.
3. **Step 3:** Preserve breathing room and sentence boundaries.
4. **Step 4:** Generate reviewable cut decisions before removing content.
5. **Step 5:** Recheck synchronization and natural flow.

## Tools and integration
Relevant options: Silero VAD; auto-editor; FFmpeg. These are candidate tools **not bundled or guaranteed available**. Confirm runtime and versions before using. Prefer low-cost preview renders, non-destructive edits, reproducible timecodes, and verified paths.

## Output contract
Return: Candidate silence cuts, timeline notes, preview. Always identify which elements were verified in a real render versus which are recommendations or instructions. Include timestamps where relevant and note missing or rejected assets.

## Acceptance checks
- Editorial: message, visual clarity, story, natural pacing, continuity and CTA are correct.
- Technical: dimensions, fps, duration, sync, codec, loudness and subtitle safe regions are checked when relevant.
- Brand: official logos, label text, product orientation and specified colors were not changed.
- Provenance: rights and source references are traceable.
- Risk: Never automatically discard client-approved dialogue.

## Ground rules
- Respect the user's brief and preserve all uploaded originals, brand marks and product packaging.
- For Gemini Apps/Tasks: this skill gives reusable expert instructions; it does **not** install, run or grant access to local Windows tools. Never claim to have executed FFmpeg, Python, an MCP connector or an NLE unless an actual supported tool returned a verified result.
- For Gemini CLI: inspect available executables and MCP servers, get consent before executing destructive or untrusted commands, write outputs only into a dedicated output directory, and test a short preview before final render.
- If a required tool is unavailable, produce an actionable edit plan, script or command for a connected environment instead of fabricating rendered assets.
- Check licensed media, privacy, copyright, synthetic speech permissions, and commercial model terms before delivery.

## Google AI Studio agent runtime addendum (20 November 2026)
- In Google AI Studio Agents Playground / managed agents, this skill is available only when its SKILL.md (and any referenced assets) is mounted into the agent environment under `.agents/skills/`. The model should select it only for matching tasks.
- In Google AI Studio Build mode, this document is *project reference material*; importing it does not register an account-level Skill or guarantee automatic loading. Ask the Build agent to inspect `AGENTS.md` and load relevant files as needed.
- Verify actual tool availability, network permission, file access and execution success. Do not claim a render, test, deployment, browser action, SDK installation, or access to Windows software without observed evidence.
- Never delete existing source files or overwrite project assets without explicit approval; preserve logos, brand details and contracts.
