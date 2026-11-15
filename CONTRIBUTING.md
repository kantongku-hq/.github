# Contributing

## Workflow
1. Pick one issue from the GitHub Project (status `Ready`).
2. Create a branch from `main`: `feat/<issue-number>-<slug>` (also `fix/`, `chore/`, `docs/`).
3. Work in small commits and run the tests locally.
4. Open a pull request using the template and link the issue with `Closes #n`.
5. Merge once CI is green and the review is done.

## Commits
Conventional Commits: `<type>(<scope>): <summary>`.

| Type | Used for |
|---|---|
| `feat` | A new feature |
| `fix` | A bug fix |
| `docs` | Documentation |
| `test` | Tests |
| `chore` | Maintenance and configuration |
| `refactor` | A structural change with no behavior change |
| `ci` | Pipelines |

## Branches and protection
- `main` is protected: changes land only through a pull request with green CI.
- One branch per issue.
- Squash merge only; the branch is deleted after merging.

## Labels
- `type:` feature, bug, chore, docs, adr, feedback
- `area:` api, web, iac, hub

## Milestones and the project board
- Milestones are named `F<phase>-M<number> <name>` and are identical across the repositories involved.
- Project fields: `Phase`, `Estimate`, `Actual`, `Priority`, `Status`.

## Language
- Code, comments, commits, issues, pull requests, and READMEs: English.
- Product documentation in the hub: Indonesian.

## Running locally
Each repository's README describes how to run it from scratch.

## Secrets
Never commit secrets. Use environment variables and provide an `.env.example` without values.
