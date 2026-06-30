# TestApp

A minimal repo to test automatic versioning with GitHub Actions.

## How to test

Open a PR against `main` with one of these in the **PR title**:

- No keyword → patch bump (0.0.1)
- `#minor` → minor bump (0.1.0)
- `#major` → major bump (1.0.0)

another test

test
When the PR is opened/updated/retitled, a workflow bumps `package.json`
and commits the new version to the **PR's source branch** (so the bump is
part of the merged history). If you change the PR title, the previous
bump commit by the bot is amended.

When the PR is merged into `main` (normal merge — full history preserved):

- Minor / major bumps are tagged `vX.Y.Z`.
- Major bumps additionally create a GitHub Release.
- The 10 most recent tags are kept; older tags are pruned.

Change 1
Change 2
Change 3fe
dvs

Minor Testfe
major
fe
testing
tests
prune
