
```md
# SoftwareSeva Starter Kit

A practical starter kit for building thoughtful, maintainable, privacy-conscious software with a modern edge stack.

This repository is the front door for the SoftwareSeva engineering ecosystem. It collects project conventions, setup instructions, dependency policies, design guidance, and Codex workflows used across SoftwareSeva projects.

## Stack

- Cloudflare Workers / Pages
- Hono
- D1, R2, KV, Queues
- React
- Tailwind CSS
- shadcn/ui
- Flutter
- Cupertino-first mobile UI
- Codex-assisted development

## What this contains

```text
starter-kit/
  AGENTS.md
  DESIGN_SYSTEM.md
  PACKAGE_POLICY.md
  CODEX_SETUP.md
  REUSABILITY_POLICY.md
  templates/
  scripts/
```

## Principles

- Keep projects small, clear, and composable.
- Prefer boring, stable dependencies.
- Extract reusable code into shared packages.
- Use Cloudflare for simple, globally distributed infrastructure.
- Use Flutter for polished mobile apps.
- Use React + shadcn/ui for admin and dashboard interfaces.
- Use Codex with clear project rules, not vague wishes.

## Getting started

Clone this repository:

```bash
git clone https://github.com/softwareseva/starter-kit.git
```

Copy the relevant files into a new project:

```bash
cp AGENTS.md ../my-project/
cp DESIGN_SYSTEM.md ../my-project/
cp PACKAGE_POLICY.md ../my-project/
```

Then adapt the project-specific sections.

## Suggested use with Codex

Every project should contain an `AGENTS.md` file. Codex should read it before planning or editing code.

Recommended prompt:

```text
Read AGENTS.md, DESIGN_SYSTEM.md, and PACKAGE_POLICY.md first. Follow the project conventions. Prefer small diffs. Before adding a dependency, verify that it is latest stable and actively maintained.
```