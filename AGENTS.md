# AGENTS.md

Context for AI agents working in this repository.

This is the BuildWarden vz driver (`buildwarden/buildwarden-driver-vz`), a component of the
componentization program. Its design, and the standards it follows until it
has its own, live in
[`buildwarden/buildwarden`](https://github.com/buildwarden/buildwarden):

- the program: `docs/design/componentization.md` and
  `docs/design/program-north-star.md`;
- the standards: `docs/development/README.md`;
- the Loop Contract (LOOP-01 to LOOP-09), the rules the development loop runs
  under in every repository it works in: `docs/development/loop-contract.md`,
  until it moves to
  [`buildwarden/buildwarden-ai-workflow`](https://github.com/buildwarden/buildwarden-ai-workflow), the
  loop's repository.

This repository is not adopted yet: it has no loop profile (PROFILE-01) until
its phase starts.

## Working here

- `program/componentization` is the program trunk. It is not a trunk: it moves only by
  merged pull requests, and no agent pushes to it directly, force-pushes it or
  deletes it.
- Never push `main`, force-push, or delete a remote branch (FLOW-16, FLOW-17).
- Agent sessions are recorded only to `buildwarden/buildwarden-sessions` (FLOW-18):
  `.entire/settings.json` names it, and the `sessions-private` check enforces
  it.
