# PROJECT_NAME

> One-sentence description of what this project does.

**Status:** planning.

## How this project is built

This project is written by [Claude](https://claude.ai/code), Anthropic's AI
coding assistant, under the oversight of its maintainer
([@nolsen311](https://github.com/nolsen311)). Every change goes through a pull
request that the maintainer reviews, signs off under the
[Developer Certificate of Origin](CONTRIBUTING.md#developer-certificate-of-origin),
and merges. Claude never merges, never tags releases, and never signs off on
anyone's behalf. See [`CONTRIBUTING.md`](CONTRIBUTING.md) and [`CLAUDE.md`](CLAUDE.md).

Design decisions are recorded in [`docs/adr/`](docs/adr/).

## Security

See [`SECURITY.md`](SECURITY.md) to report a vulnerability.

## License

[GPL-3.0-or-later](LICENSE).

---

## Using this template

*Delete this section once the project is set up.*

1. Create the repository from the template:

   ```bash
   gh repo create nolsen311/NEW_REPO --template nolsen311/claude-project-template --public --clone
   ```

2. Run the bootstrap script once, as the repository owner. It configures
   everything a template can't copy (rulesets, security settings, the
   `release` environment):

   ```bash
   cd NEW_REPO && scripts/bootstrap.sh nolsen311/NEW_REPO
   ```

   Run with `--dry-run` first to see every change without making it. The
   script ends with any manual steps, including granting the Claude GitHub
   App access to the new repository (GitHub doesn't allow that through `gh`).

3. Replace `PROJECT_NAME` and the description above, and record the
   initial commit in [`docs/dco-remediations.md`](docs/dco-remediations.md)
   (the bootstrap script prints the entry).

4. Add language-specific CI (lint, tests, builds) and its Dependabot
   ecosystem, then add those job names to `.github/rulesets/protect-main.json`
   and re-run the bootstrap script.

   For releases by comment (ADRs 0004 and 0005), set `VERSION_FILE` in
   `.github/workflows/release-tag.yml`, and set up the release app
   ([`CONTRIBUTING.md`](CONTRIBUTING.md), "Release app"). A release workflow
   that runs on `push: tags` starts from the tags it creates.

5. Start a Claude Code session with the new repository selected.
