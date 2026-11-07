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

## 2026-11-07 (second entry)

PR #1 was merged with a merge commit instead of a squash, before this
repository was bootstrapped (so the squash-only setting was not yet applied).
The merge commit carries no sign-off, and Claude's commits from that PR
reached `main` unsquashed. Because PR #1 was not merged with a sign-off, its
entry for `a8dbdc5` (above) also takes effect only with this remediation.

| Commit | Subject |
| --- | --- |
| `a8dbdc511a66e8041b2edcb258dbfd5c1b218b64` | Initial template: DCO workflow, Claude working rules, baseline CI and bootstrap |
| `0da1fcf4bde2a4779e3039f2d23d0c22d09039ff` | Fix bootstrap.sh bugs found in the first real dry run; add tests |
| `8711ae0db00a72251cb5f8f03bcf6a1d1e6c2367` | CodeQL: grant actions: read so analysis works in private repositories |
| `63b19a29b1f920500d190fd717552148eac15a65` | Merge pull request #1 from nolsen311/claude/fix-bootstrap |
