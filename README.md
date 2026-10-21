# Skills

Curated agent skills maintained by [rozsazoltan](https://github.com/rozsazoltan).

Each skill lives in its own directory under `skills/` and follows the standard `SKILL.md` layout used by agent hosts such as [OpenCode](https://opencode.ai/) and [APM](https://github.com/microsoft/apm).

## Available skills

| Skill | Purpose |
| --- | --- |
| [`anti-slop-review`](skills/anti-slop-review/SKILL.md) | Review-only routing skill that audits code, technical prose, and UI against AI-slop patterns without changing files by default. |

## Installation

Install a skill directly with APM from this repository:

```bash
apm install rozsazoltan/skills/skills/<skill-name> --target opencode
```

For example:

```bash
apm install rozsazoltan/skills/skills/anti-slop-review --target opencode
```

Replace `<skill-name>` with a directory name from `skills/`.

## License

Licensed under the GNU Affero General Public License, version 3 or later. See [LICENSE](LICENSE).
