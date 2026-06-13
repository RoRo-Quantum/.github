# Repository Standards

Apply this checklist when adding/moving a new repo into RoRo Quantum.
Consistency keeps the org professional and easy to maintain.

## Naming

- All **lowercase**, words separated by **hyphens**: `quantum-sdk-swift`, `qpu-simulator`
- SDKs use a language suffix: `...-swift`, `...-python`, `...-js`, `...-rust`
- Tools/internal: descriptive and short.

## Every repo should have

- [ ] `README.md` — what, why, install, quick start
- [ ] `LICENSE` — for public SDKs (suggested: **MIT** or **Apache-2.0**)
- [ ] `.gitignore` — matching the language
- [ ] A meaningful `description` and **topics** (e.g. `quantum`, `sdk`, `swift`)
- [ ] Default branch: **`main`**

> `CONTRIBUTING`, `CODE_OF_CONDUCT`, `SECURITY`, and issue/PR templates come
> **automatically** from the org `.github` repo — no need to duplicate them
> unless you want to override.

## Visibility

- **Private** by default while in development (current org policy).
- Flip to **Public** only when the project is ready to ship.

## Branch protection (recommended — for `main`)

- [ ] No direct pushes without a PR
- [ ] At least **1 review** required
- [ ] CI checks (if any) must pass before merge
- [ ] No force-push to `main`

> Instead of doing this per-repo, we can apply an **org ruleset** once to cover
> all repos (Settings → Repository rulesets).

## Team access

| Team | Typical access |
|------|----------------|
| `@RoRo-Quantum/core` | admin (private + infra) |
| `@RoRo-Quantum/maintainers` | maintain / write |
| `@RoRo-Quantum/sdk` | write (public SDKs) |

## Labels

Suggested set for consistent triage: `bug`, `enhancement`, `documentation`,
`good first issue`, `help wanted`, `triage`, `question`, `wontfix`.
