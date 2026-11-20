# Gemini Apps Tasks: Verified boundaries (official Google docs, 2026-11-20)

- A Gemini Apps Skill is a folder or ZIP with a **root-level** `SKILL.md`, using lowercase hyphenated `name` metadata. It can include supported `.md`, `.txt`, `.py`, `.js`, `.json` and other supported reference files.
- Gemini Skills UI path: gemini.google.com > Customize > Skills > Create > Upload. In Gemini Task, insert `/` or `@` and select an enabled Skill.
- Skills currently have 100 MB total file-size limit. Uploaded skill scripts **cannot access external websites**.
- The Gemini Apps skill upload does **not** install FFmpeg, Python, npm dependencies, model checkpoints, Premiere or Resolve on the local Windows computer. It teaches Gemini the workflow; executing software needs a separately supported runtime or connector.
- Gemini CLI on Windows is a **different local development product**, and supports user skills at `~/.gemini/skills/<skill-name>/SKILL.md` and workspace skills at `.gemini/skills/<skill-name>/SKILL.md`; interactive `/skills list` and `/skills reload` commands check discovery.
- Skills for Gemini Apps are usable across chat and Task; one root-level SKILL.md ZIP creates **one Skill**, not 45 independent Skills in one upload.

Official sources:
- https://support.google.com/gemini/answer/17094296
- https://support.google.com/gemini/answer/17094507
- https://geminicli.com/docs/cli/skills/
- https://geminicli.com/docs/get-started/installation/
- https://geminicli.com/docs/tools/mcp-server/
