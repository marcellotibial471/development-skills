# Development Skills

[简体中文](./README.zh-CN.md) | English

Reusable development workflow skills for end-to-end software delivery.

This repository packages a development workflow as reusable agent skills. It helps move a feature from requirement definition to tested implementation with a consistent process.

## Included Skills

- `spec`
- `plan`
- `implement`
- `review`
- `test`

## Installation

### Option A: skills.sh

Install a single skill from this repository using `skills.sh`:

```bash
npx skills add https://github.com/SimpleEve/development-skills --skill spec
npx skills add https://github.com/SimpleEve/development-skills --skill plan
npx skills add https://github.com/SimpleEve/development-skills --skill implement
npx skills add https://github.com/SimpleEve/development-skills --skill review
npx skills add https://github.com/SimpleEve/development-skills --skill test
```

### Option B: Claude Code Plugin

Install the full plugin through Claude Code marketplace:

```bash
/plugin marketplace add SimpleEve/development-skills
/plugin install development-skills@simpleeve-development-skills
```

### Option C: Manual Install

```bash
git clone git@github.com:SimpleEve/development-skills.git
```

Then copy one or more skill folders into the local skills directory used by your host application, and restart the host.

## Recommendation

These skills were generalized from a set of project-specific internal skills.

The original versions contained conventions, constraints, and workflow details tied to a real project, so they were not suitable for direct public sharing. This repository keeps the core workflow, but intentionally removes project-specific assumptions.

For best results, treat these skills as a starting point rather than a final drop-in package. After installing them, it is recommended to use AI to review the skill content against your own project and then add back the constraints, terminology, directory conventions, architecture rules, and workflow expectations that are specific to your environment.

## Usage Examples

- "Write a spec for a new notification system"
- "Create an implementation plan for this feature"
- "Implement the approved plan"
- "Review this code against the spec and plan"
- "Write tests and produce a test report"

## License

MIT. See [LICENSE](./LICENSE).
