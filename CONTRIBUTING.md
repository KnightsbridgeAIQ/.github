# Contributing

Thanks for your interest in the KXCO stack. These packages run in production
at KXCO, so we keep surfaces small and the bar for changes high.

**What we welcome:** bug fixes, test-vector additions, documentation
improvements, and reproducible issue reports.

**What we generally don't merge:** new features, API changes, or new
dependencies from external contributors. If you need a capability, open an
issue describing the use case first — we'd rather design it with you than
review a large unsolicited PR.

## Security issues

Never open a public issue for a vulnerability. Use the repository's
**Security → Report a vulnerability** tab, or email **security@kxco.ai**.
See [SECURITY.md](SECURITY.md).

## Ground rules

1. One logical change per pull request.
2. Every behaviour change needs a test. Cryptographic changes need test
   vectors — code without vectors won't be merged.
3. CI must pass and a code owner must review before merge.
4. Commit messages use Conventional Commits prefixes
   (`feat:`, `fix:`, `docs:`, `deps:`, `ci:`, `chore:`).
5. No new runtime dependencies without prior discussion in an issue.
6. Company code lives in this organization — never in personal accounts.
   This applies to employees and contractors alike.

## Deprecation policy

When a repository or package reaches end of life we do not delete it or let
it rot. We prefix its description with "DEPRECATED", point to the successor
in the description and README, then archive the repository. Archived code
stays browsable forever.

## Questions

Open an issue on the relevant repository, or email **hello@kxco.ai**.
