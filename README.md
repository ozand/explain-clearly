# Explain Clearly

English | [Русский](README.ru.md)

![Abstract illustration for Explain Clearly](assets/explain-clearly.jpg)

`explain-clearly` is an [Agent Skill](https://agentskills.io/) for answering requests
to make an explanation clearer. It aims to help a reader understand the relevant mechanism and
reason without losing important facts, uncertainty, or safety boundaries. It applies
to technical and nontechnical topics and adapts to the audience and depth requested.

## Scope

The skill offers writing guidance: identify the reader's question, explain the needed
causal link, ground it in a useful example, and distinguish evidence from assumptions
and unknowns. It does not guarantee correctness or comprehension, replace subject-matter
expertise, or prescribe a project-status process. Its self-review is not evidence that
human readers understood. Selection and installation behavior depend on the agent.

## Install

This repository root is the skill package: `SKILL.md` and its `references/` directory
belong together. Clone the repository, then copy the repository contents into the
skill location supported by your agent. Consult that agent's documentation for the
location and any required activation or configuration. There is no universal install
command or automatic activation guarantee.

An agent that supports manually loading skill instructions can also be given the
contents of `SKILL.md`; keep `references/` alongside it if you want the examples and
source notes available. Agent-specific installation and loading conventions vary.

## For AI agents

A repository URL alone does not specify whether the user wants to use or install a
skill. Follow the user's request and the host's instructions:

1. Read `SKILL.md` and the referenced files relevant to the request. To use it for
   one conversation, apply the guidance without changing the host's configuration.
2. For installation, consult the host's documentation to identify its supported
   skill location and scope. Copy `SKILL.md` **and** `references/` together; preserve
   existing files and do not overwrite another skill without permission.
3. Report the installation location and any required reload. Do not claim that a
   running agent discovered or activated the skill unless that was actually checked.

## Example requests

- English: “Explain why this page may still show the old image after I replaced it.”
- English: “I don't understand this result. Explain what the check establishes and what
  it does not establish.”
- Russian: «Объясни простыми словами, почему страница может показывать старую картинку
  после замены.»
- Russian: «Я не понимаю этот результат. Объясни, что именно подтверждает проверка и
  чего она не подтверждает.»

## Before and after

Before: “Cache invalidation caused stale asset delivery.”

After: “Your browser may have saved an earlier copy of the picture and reused it
instead of downloading the replacement. Those saved files are called the browser
cache. Clearing them can make the browser download the picture again, but it will not
fix an image that is wrong on the site itself. This is one possible explanation, not a
diagnosis from the symptom alone.”

The rewrite shows one possible mechanism and its limit; it does not establish what
caused any particular user's issue.

## License

Released under the [MIT License](LICENSE).

## References

- [Examples](references/examples.md) — three fictional, contextual illustrations.
- [Sources](references/sources.md) — practitioner writing advice behind parts of the
  approach; not controlled evidence or a claim of universal effectiveness.
