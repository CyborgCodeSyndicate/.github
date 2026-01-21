# Contributing

Thanks for your interest in this project.

This organization maintains multiple repositories and modules. Each repository may include additional contribution rules in its `README.md`. If repo-specific rules conflict with this document, **the repository rules win**.

---

## Code of Conduct

By participating, you agree to uphold our **Code of Conduct**. Please read `CODE_OF_CONDUCT.md` before engaging in issues, discussions, or reviews.

---

## Security

**Do not report security vulnerabilities via public issues or pull requests.**

Please follow the instructions in `SECURITY.md` for responsible disclosure. Security reports posted publicly may be removed to protect users.

---

## Support and Questions

If you need help using the project, have questions, or want to report a bug, see `SUPPORT.md`.

When requesting help, include:
- Repository name + module (if applicable)
- Version / commit hash
- Expected vs actual behavior
- Minimal reproduction steps
- Environment details (OS, Java version, Maven/Gradle versions)
- Relevant logs (remove secrets)

---

## Contribution Policy (Members Only)

### No external contributions
**This project does not accept external contributions.**  
Pull requests, direct commits, and code changes are restricted to **members of the organization** with appropriate access.

If you are not a member, you can still contribute by:
- Reporting bugs with reproducible steps
- Suggesting improvements with clear use-cases and constraints
- Sharing integration feedback (edge cases, platform details, compatibility notes)

Requests for membership or access are handled via the channels described in `SUPPORT.md`.

---

## Pull Request Validator (Required)

All pull requests must pass the **Pull Request Validator** pipeline checks.  
If the PR Validator passes, the change is considered compliant and **good to go**. If it fails, the PR is not eligible for merge.

### Run the same validation locally
Before opening a PR (or when debugging CI failures), run the same command used by the validator:

```bash
mvn clean verify -Ppr-validator
```

If the repository uses the Maven Wrapper, prefer:

```bash
./mvnw clean verify -Ppr-validator
```

> CI is the source of truth. Local runs are to reduce iteration time and match the validator as closely as possible.

---

## Workflow for Organization Members

### 1) Create/confirm a tracked work item
Before writing code, ensure the work is tracked (issue / discussion / internal ticket) with:
- Clear scope
- Acceptance criteria
- Compatibility expectations (breaking vs non-breaking)

### 2) Branch naming
Use short, descriptive branches:
- `feature/<short-scope>`
- `fix/<short-scope>`
- `docs/<short-scope>`
- `chore/<short-scope>`

### 3) Commit messages
Keep commits focused and reviewable. Conventional messages are recommended:
- `feat: ...`
- `fix: ...`
- `docs: ...`
- `refactor: ...`
- `test: ...`
- `chore: ...`

---

## Pull Request Guidelines (Members)

A good PR includes:
- What changed and why
- Link to the tracked work item
- Tests added/updated (or explanation if not applicable)
- Docs updates when user-facing behavior changes
- Migration notes if there are breaking changes

### PR checklist
- [ ] Scope is minimal and aligned with acceptance criteria
- [ ] PR Validator command executed locally (recommended): `mvn clean verify -Ppr-validator`
- [ ] Tests added/updated and passing
- [ ] No secrets committed (tokens, keys, credentials)
- [ ] Documentation updated where necessary
- [ ] Backward compatibility considered; version impact noted
- [ ] PR Validator pipeline checks pass in CI

### Review expectations
- Be responsive to feedback
- Prefer small incremental improvements over large rewrites
- Keep discussions technical and respectful

---

## Documentation Standards

If you add or change functionality, update documentation accordingly:
- README usage snippets
- Configuration options
- Examples / sample projects
- Any “getting started” steps impacted

Write docs for users first: **how to use it**, then (optionally) how it works.

---

## License

By contributing, you agree that your contributions may be redistributed under the repository’s license. If a repository requires additional agreements, it will be documented in that repository.

---

## Thank you

Bug reports, feedback, and high-quality internal contributions help keep the ecosystem stable and reliable.
