# Contributing to Sparfuchs Projects

Thanks for considering a contribution. This document covers the essentials — how we work, what we'll merge quickly, and what we'll ask you to rethink. It applies to every public repository under the [Sparfuchs-corporation](https://github.com/Sparfuchs-corporation) organization unless a specific repo overrides a section with its own `CONTRIBUTING.md`.

---

## Our Philosophy

Sparfuchs projects support the **Aegis Methodology** — governing agentic AI with quality, visibility, and control. That shapes what we merge:

- **Evidence over opinion.** Bugs come with reproductions. Features come with motivation. "It would be nice if" is a Discussion, not a PR.
- **Determinism where possible, LLM where necessary.** If a check can be a script, it should be a script. Don't reach for an LLM when a regex will do.
- **Fail-closed by default.** New policies, permissions, and autonomy grants start restrictive. Earn the relaxation with evidence.
- **Audit trail or it didn't happen.** Agent actions, config changes, and classification decisions must be traceable.

If a contribution runs against these, we'll say so early and explain why.

---

## Before You Start

1. **Search existing issues and discussions** — your question or idea may already be in flight.
2. **For anything non-trivial, open an issue first.** We'd rather redirect you before you've written the code than after.
3. **Check the repo-specific `README.md` and any `docs/` folder** — some projects have their own architectural constraints.

---

## Ways to Contribute

- 🐛 **Bug reports** — use the bug issue template; include reproduction steps, environment, and expected vs. actual behavior
- ✨ **Feature proposals** — open a Discussion first. PRs without a prior issue or Discussion may be closed pending that conversation
- 📚 **Documentation** — typos, clarifications, and examples are always welcome; no issue needed for small fixes
- 🧪 **Benchmarks & evals** — if you've stress-tested one of our agents or canaries, we want the data
- 🔌 **Adapters & integrations** — new CLI adapters, CI integrations, and provider wrappers should follow the declared-fallback-chain pattern; see the relevant repo for the contract
- 🔒 **Security issues** — **do not file public issues.** Email **security@sparfuchs-pro.com**. See [SECURITY.md](./SECURITY.md)

---

## Pull Request Process

1. **Fork and branch.** Branch names: `feat/<short-desc>`, `fix/<issue-number>`, `docs/<short-desc>`.
2. **One logical change per PR.** Splitting is cheap; un-splitting is expensive.
3. **Tests.** New behavior ships with tests. Bug fixes ship with a regression test that fails without the fix.
4. **Lint and format before pushing.** Every repo has CI; run it locally first.
5. **Write a real PR description.** Include: what changed, why, how you tested it, and any trade-offs you considered and rejected.
6. **Link the issue.** `Closes #123` or `Refs #123` in the description.
7. **Be patient but not silent.** We review weekly. If a review stalls beyond a week, ping the PR politely.

### What gets merged fast

- Small, focused PRs with tests and a clear rationale
- Documentation improvements that reduce reader friction
- Bug fixes with regression tests
- Additions that follow existing patterns rather than inventing new ones

### What gets pushed back

- Large refactors without a prior design discussion
- Dependencies added without justification
- New LLM calls where a script runner would suffice
- Changes that weaken fail-closed defaults or audit trails
- Code without tests in repos that have test suites

---

## Code Style

- Follow the existing style in each repo. If the repo has linter configs, those are the source of truth.
- TypeScript projects use strict mode. Don't disable it locally.
- Names should describe behavior, not implementation.
- Comments explain **why**, not what. If the what isn't obvious, rewrite the code before writing the comment.

---

## Commit Messages

We use Conventional Commits:

```
feat(sparfuchs-qa): add semantic-diff-reviewer runner
fix(agentforge): prevent token budget bypass on paused agents
docs(aegis): clarify 8-factor classification example
test(business-forge): cover emergent problem discovery across all six phases
```

Types we use: `feat`, `fix`, `docs`, `test`, `refactor`, `chore`, `perf`, `ci`, `build`.

---

## Licensing

By submitting a contribution, you agree that your contribution is licensed under the same terms as the repository it targets (see each repo's `LICENSE`). For contributions to repositories carrying patented methods, you additionally agree to the terms in that repository's `CONTRIBUTING.md` or `CLA.md`, if present.

---

## Code of Conduct

Be direct, be kind, be technical. Disagreement is expected; disrespect is not. Violations are handled by the maintainers at their discretion, up to and including blocks from the organization. Report issues to **conduct@sparfuchs-pro.com**.

---

## Getting Help

- **GitHub Discussions** — the fastest way to reach maintainers and other contributors
- **Email** — hello@sparfuchs-pro.com for general questions; security@sparfuchs-pro.com for anything sensitive
- **Docs** — each repo's `README.md` and `docs/` folder

Thank you for helping us build the governance layer for agentic AI.

— The Sparfuchs team

<sub>© 2026 Sparfuchs Corporation. All rights reserved.</sub>
