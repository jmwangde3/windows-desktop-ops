# windows-desktop-ops

Small routing and safety Skill for native Windows desktop operations. It is **not** a replacement for the upstream `cua-driver` Skill or the `agent-browser` Skill.

## Install

Place `SKILL.md` at the root of an enabled Skill folder. Assign it only to projects/scenarios that need native Windows UI control. Keep `cua-driver` available separately.

## Boundaries

- Native app GUI: `cua-driver`.
- Web-page interaction: `agent-browser`.
- File/CLI/API tasks: prefer direct commands.
- Foreground escalation requires permission; unsupported routes are reported, not bypassed.

No executables, dependencies, credentials, or external configuration are bundled.
