# Third-party skill attribution

This repository vendors the following MIT-licensed skill packages into Antigravity's `skills/` and `agents/` discovery layout. Their original licenses are preserved in `third-party-licenses/`.

| Package | Upstream | Included content | License |
|---|---|---|---|
| Agent Skills | https://github.com/aachauhan17achv/agent-skills | 25 skills, 4 agent templates, and shared references | MIT — Addy Osmani |
| Planning with Files | https://github.com/aachauhan17achv/planning-with-files | Skill, scripts, references, examples, templates, and eval fixture | MIT — Ahmad Adi |
| Taste Skill | https://github.com/aachauhan17achv/taste-skill | Frontend design skill, scripts, library data, assets, references, and eval fixture | MIT — Leonxlnx |

The copies are intentionally kept in separate directories so updates and removals can be traced to their original projects. Review each upstream project before updating these vendored copies.

## Antigravity adaptation

The Planning with Files skill's Claude Code-specific lifecycle-hook frontmatter is not supported by this plugin adapter and has been removed. Its skill workflow and helper scripts remain included; automatic Claude lifecycle interception is not claimed or configured.
