# DCO remediations

Commits on `main` that landed without a `Signed-off-by:` line, and the later
commit in which the maintainer signed off on them. History on `main` is never
rewritten, so a missing sign-off is fixed by a follow-up commit listed here.

A remediation takes effect when the commit that adds its entry is merged with
the maintainer's `Signed-off-by:` line. That sign-off certifies the Developer
Certificate of Origin 1.1 (see [`CONTRIBUTING.md`](../CONTRIBUTING.md)) for each
commit listed in the entry, as if it had been signed off at merge.

<!--
Template for an entry:

## YYYY-MM-DD

Why these commits lack a sign-off (for example: the initial commit created
from the project template).

| Commit | Subject |
| --- | --- |
| `<full sha>` | <subject> |
-->

## 2026-11-07

The initial template commit, pushed directly to the empty repository before
branch protection existed (the one documented exception to the pull-request rule).

| Commit | Subject |
| --- | --- |
| `a8dbdc511a66e8041b2edcb258dbfd5c1b218b64` | Initial template: DCO workflow, Claude working rules, baseline CI and bootstrap |
