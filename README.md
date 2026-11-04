# lesslop

A catalog of agent skills and tools. Less generic output, more care for writing and interfaces.

This repository provides links to original projects and installation guidance. External skills are linked to their upstream repositories. Skills hosted in this repository live in `skills/`.

## Catalog

| Project | Purpose | Source |
| --- | --- | --- |
| lesslop-presentation | Create an HTML presentation and a finished PPTX | [skills/lesslop-presentation](skills/lesslop-presentation) |
| frontend-slides | Build HTML slides | [zarazhangrui/frontend-slides](https://github.com/zarazhangrui/frontend-slides) |
| humanizer | Edit prose and remove formulaic AI writing | [blader/humanizer](https://github.com/blader/humanizer) |
| pptx | Create, edit, and validate PowerPoint files | [anthropics/skills → pptx](https://github.com/anthropics/skills/tree/main/skills/pptx) |
| calculate-tax | Calculate an invoice for a target amount after tax; default rate: 7% | [skills/calculate-tax](skills/calculate-tax) |
| sasha | Russian interface copy and documentation | [mishanaer/deslop → sasha](https://github.com/mishanaer/deslop/tree/main/sasha) |
| unslop | Refine interfaces with generic AI design | [heydamir/unslop](https://github.com/heydamir/unslop) |
| impeccable | Design, review, and polish interfaces | [pbakaus/impeccable](https://github.com/pbakaus/impeccable) |
| MarkItDown | Convert documents and files to Markdown; a Python tool | [microsoft/markitdown](https://github.com/microsoft/markitdown) |
| UI UX Pro Max | Find UI/UX and design system solutions | [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) |

Machine-readable catalog: [catalog.json](catalog.json). Agent instructions: [AGENTS.md](AGENTS.md).

## Install with an agent

Give your agent this prompt:

```text
Read https://github.com/glkhv/lesslop, AGENTS.md, and catalog.json.
Install the listed skills and MarkItDown for the target agent.
Use the current installation instructions from each original project.
Ask which platform and installation scope to use if they are unknown.
Validate the result and report installed versions and sources.
```

You can also select individual projects: “Install sasha and unslop from glkhv/lesslop for Codex.”

Cloning lesslop does not install anything. Source links let an agent retrieve the current version during installation or an update; they do not update local files automatically. To update, ask your agent to check the sources again and update the selected projects.

## Installation guidance

Check the source project's current README before running commands: paths and instructions may change.

- **lesslop-presentation:** install the complete `skills/lesslop-presentation` directory. Required dependencies: `frontend-slides`, `ui-ux-pro-max`, `impeccable`, `humanizer`, and `pptx`. Install any missing dependencies from this catalog.
- **frontend-slides, humanizer, pptx:** follow their current upstream instructions and include all supporting files. Observe the upstream license for `pptx`.
- **calculate-tax:** install the complete `skills/calculate-tax` directory from this repository, including `agents/openai.yaml`. Example: “Install calculate-tax from glkhv/lesslop for Codex.”
- **sasha:** install the complete `sasha` directory from `mishanaer/deslop`, including supporting files.
- **unslop:** install the complete `skills/unslop` directory from `heydamir/unslop`.
- **impeccable:** use the official installer, `npx impeccable@latest install`, and select your agent and installation scope. Follow the current upstream instructions for updates.
- **UI UX Pro Max:** use the official CLI; for example, `npx ui-ux-pro-max-cli@latest init --ai codex` installs for Codex in the current project. Choose the appropriate option from the upstream README for other platforms.
- **MarkItDown:** install it as a tool in a separate Python environment following its README. Example: `python -m pip install --upgrade 'markitdown[all]'`. Select dependencies for the formats you need; this is not a skill directory.

Some skills overlap. Choose the appropriate skill for the task instead of running every review unnecessarily.

## Attribution

Listed projects belong to their respective authors. Their licenses and terms are available in the original repositories. lesslop is an independent collection, not an official bundle from those projects.
