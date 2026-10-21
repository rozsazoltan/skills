# Skills

Curated agent skills maintained by [rozsazoltan](https://github.com/rozsazoltan).

Each skill is its own top-level directory in this repository and follows the standard `SKILL.md` layout used by agent hosts such as [OpenCode](https://opencode.ai/) and [APM](https://github.com/microsoft/apm).

## Installation

Install a skill directly with APM:

```bash
apm install rozsazoltan/skills/<skill-name> --target opencode
```

Replace `<skill-name>` with the skill directory name. A skill that needs other skills declares them in its own `apm.yml`, so installing it installs everything it depends on.

## License

Licensed under the GNU Affero General Public License, version 3 or later. See [LICENSE](LICENSE).
