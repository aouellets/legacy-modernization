# Legacy Modernization & Migration

**For engineers in legacy code: modernize incrementally, no big-bang rewrite.** — built in-house by [Skill&nbsp;Me](https://skillme.dev).

Reach for this when you inherit a business-critical codebase that has to keep running while you drag it onto a modern stack. Plan a strangler-fig migration that runs old and new side by side, carve one safe bounded-context seam out of a monolith, drive major framework and language-version upgrades as small reversible CI-gated PRs, recover the business rules buried in tangled code, pin current behavior with characterization tests before you touch it, audit dependency risk as you upgrade, and delete dead code with evidence — so nothing breaks while everything moves.

⭐ **If this is useful, star the repo** — it's how we gauge what to build next.

## Install

- **From the catalog:** [skillme.dev/pack/legacy-modernization](https://skillme.dev/pack/legacy-modernization) — install the whole pack into Claude in one step.
- **With the skills CLI:** `npx skills add aouellets/legacy-modernization`
- **Manually:** copy any `skills/<slug>/SKILL.md` into your Claude skills directory.

## Skills in this pack

- **[Strangler Fig Planner](skills/strangler-fig-planner/SKILL.md)** — Produces an incremental migration plan that runs a legacy and a new system side by side behind a routing seam, slicing and sequencing whole capabilities so the old system stays live until its last route is cut.
- **[Framework Upgrader](skills/framework-upgrader/SKILL.md)** — Drives a major-version framework bump as a sequence of small, reversible, CI-gated PRs using official codemods and changelog diffing while keeping the app green.
- **[Language Version Migrator](skills/language-version-migrator/SKILL.md)** — Ports a codebase across a breaking language or runtime version using compatibility shims, automated transforms, and old-vs-new verification.
- **[Business Rule Extractor](skills/business-rule-extractor/SKILL.md)** — Produces a documented inventory of the implicit business rules, edge cases, and bug-as-feature behaviors that tangled code encodes, with real input-to-output examples, so a rewrite preserves behavior.
- **[Characterization Test Writer](skills/characterization-test-writer/SKILL.md)** — Writes pinning and characterization tests that lock in the current behavior of untested legacy code before a refactor, so any later behavior change trips an alarm.
- **[Dead Code Eliminator](skills/dead-code-eliminator/SKILL.md)** — Proves code is unreachable with converging evidence, then removes it and its tests, fixtures, and flags in reversible slices without breaking dynamic callers.
- **[Monolith Decomposer](skills/monolith-decomposer/SKILL.md)** — Finds and sequences one bounded-context seam to extract from a monolith, gated on dependency, data-ownership, and transaction-boundary evidence, and produces an incremental strangler extraction plan.
- **[Dependency Risk Audit](skills/dependency-risk-audit/SKILL.md)** — Assesses third-party dependency risk across CVEs, maintenance health, license exposure, and supply-chain hygiene.
- **[TDD Expert](skills/tdd-expert/SKILL.md)** — Enforces Red-Green-Refactor discipline: write the failing test first, then the minimum code to pass it.

## License

MIT — see [LICENSE](LICENSE). Skills are portable `SKILL.md` files; the canonical
copies live in the [Skill&nbsp;Me catalog](https://skillme.dev).
