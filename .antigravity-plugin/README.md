# API Anything — Antigravity plugin

This repository now supports Antigravity as well as its existing Claude Code plugin.

## Included capability packs

- **API Anything** — discover, learn, call, verify, share, and repair website operations through the existing MCP server.
- **Agent Skills** — the 25 engineering lifecycle skills, 4 specialist agent templates, and shared reference checklists.
- **Planning with Files** — persistent project plans, findings, progress ledgers, templates, and helper scripts. The Claude Code lifecycle hooks are intentionally not enabled in Antigravity; invoke the skill when useful.
- **Taste Skill** — frontend art direction, design research assets, browser inspection, and iterative visual QA. This is a specialist skill for UI and web-design tasks.

## Install

```bash
agy plugin install https://github.com/aachauhan17achv/api-anything.git
```

Check the installed plugin:

```bash
agy plugin list
```

For a local checkout, validate before installing:

```bash
agy plugin validate --strict .
agy plugin install .
```

The API Anything MCP server is declared in the repository-root `mcp_config.json`. It starts with Node.js and npx; the first launch may download the package.

## Notes

- Skills are discovered on demand from `skills/<skill-name>/SKILL.md`.
- Planning with Files is adapted for explicit Antigravity invocation. Claude-specific automatic hooks are not carried over.
- Taste Skill's scripts require Node.js 22+ and an installed Chrome, Edge, or Chromium browser. Some asset discovery steps need network access.
- Third-party source notices and origins are recorded in `THIRD_PARTY_SKILLS.md` and `third-party-licenses/`.
