# Kibana Agent Skills Index
Generated from repository contents under `.agents/skills/`.

## api-authz
Description: Kibana API route authorization patterns. Use when configuring route security, working with requiredPrivileges, using authzResult for privilege-based branching, opting out of authorization, or naming custom privileges.
Files:
- .agents/skills/api-authz/SKILL.md

## branch-readiness-checks
Description: Validate branch readiness before push or PR using base-diff and local-change checks.
Files:
- .agents/skills/branch-readiness-checks/SKILL.md

## buildkite-logs
Description: Fetch and analyse Buildkite CI logs for the elastic/kibana repo. Provides helpers to retrieve build/job logs by build number or PR number, summarise failures, and inspect artifacts. Use when the user asks about CI failures, Buildkite logs, a failing build, a red CI, build artifacts, or mentions a Buildkite URL or PR number in the context of CI.
Files:
- .agents/skills/buildkite-logs/SKILL.md

## codeql
Description: Work with CodeQL in Kibana — write, test, and debug custom queries locally, fetch scan results from GitHub, and validate inline suppression comments. Use when writing or debugging CodeQL queries, running CodeQL unit tests, analyzing SARIF results, fetching scan results, or checking codeql suppression justifications.
Files:
- .agents/skills/codeql/SKILL.md

## cypress-to-scout-migration
Description: Migrate Kibana Cypress E2E tests (.cy.ts) to Scout (Playwright). Applies to any Kibana plugin or solution. Includes triage gates (duplicate detection, layer analysis, value assessment), Cypress-to-Scout pattern mapping, data cleanup audit, and PR workflow. Use when: (1) migrating a Cypress test to Scout, (2) converting .cy.ts to .spec.ts, (3) planning a Cypress-to-Scout migration batch, (4) rewriting Cypress screens/tasks as Scout page objects, (5) asked "how do I move this Cypress test to Scout/Playwright", (6) asked about differences between Cypress and Scout.
Files:
- .agents/skills/cypress-to-scout-migration/SKILL.md
- .agents/skills/cypress-to-scout-migration/references/cypress-vs-scout-differences.md
- .agents/skills/cypress-to-scout-migration/references/example-migration.md
- .agents/skills/cypress-to-scout-migration/references/flakiness-risk-patterns.md
- .agents/skills/cypress-to-scout-migration/references/migration-best-practices.md

## debug-oas
Description: Use when debugging OpenAPI (OAS) issues for a specific API area in Kibana by scoping validation output with one or more --path filters, then separating structural invalid-OAS failures from quality or documentation gaps such as missing descriptions.
Files:
- .agents/skills/debug-oas/SKILL.md

## encrypted-saved-objects
Description: Encrypted Saved Objects (ESO) in Kibana — registration, AAD attribute choices, partial update safety, model version migrations with createModelVersion, canEncrypt checks, and Serverless constraints. Use when creating, modifying, or working with ESO types.
Files:
- .agents/skills/encrypted-saved-objects/SKILL.md

## enzyme-to-rtl
Description: Migrate Enzyme tests to React Testing Library (RTL). Use when converting shallow/mount enzyme tests to RTL render, replacing enzyme selectors with RTL queries, updating snapshot tests, or when the user mentions enzyme migration, RTL migration, or react-testing-library.
Files:
- .agents/skills/enzyme-to-rtl/SKILL.md

## evals-create-suite
Description: Scaffold a new LLM evaluation suite package with Playwright config, evaluate fixture, and package files. Use when creating a new eval suite, adding an evals package for a plugin, or setting up the boilerplate for offline LLM evaluations.
Files:
- .agents/skills/evals-create-suite/SKILL.md

## evals-write-spec
Description: Write LLM evaluation spec files with datasets, tasks, and evaluators using the @kbn/evals Playwright fixture. Use when authoring new eval specs, adding datasets or evaluators, or debugging evaluation test failures.
Files:
- .agents/skills/evals-write-spec/SKILL.md
- .agents/skills/evals-write-spec/references/evaluator-patterns.md

## fix-package-docs
Description: Fix API documentation issues in a Kibana plugin or package. Use when asked to fix, improve, or add JSDoc/API documentation for a Kibana plugin or package, or when check_package_docs validation fails.
Files:
- .agents/skills/fix-package-docs/SKILL.md

## ftr-testing
Description: Deep reference for the Kibana Functional Test Runner (FTR). Use when reading, analyzing, debugging, or reviewing FTR tests, including config anatomy, services, page objects, loadTestFile patterns, data loading, tags, CI wiring, and common FTR idioms.
Files:
- .agents/skills/ftr-testing/SKILL.md

## gh-create-issue
Description: Create a new GitHub issue (feature request or bug report) by gathering an unstructured description from the user, classifying it, filling out the appropriate Kibana template, interviewing the user to improve any weak sections, and filing the issue via the GitHub CLI.
Files:
- .agents/skills/gh-create-issue/SKILL.md

## gh-enhance-issue
Description: Fetch a GitHub issue by number or URL and reformat it according to the Kibana bug report or feature request template. Classifies the issue type automatically, then rewrites the body and updates it via the GitHub CLI.
Files:
- .agents/skills/gh-enhance-issue/SKILL.md

## kibana-api
Description: Shared utilities for interacting with a local Kibana instance. Provides auto-detection of Kibana URL and auth, and a kibana_curl wrapper.
Files:
- .agents/skills/kibana-api/SKILL.md

## kibana-privilege-deprecation
Description: Implement and review Kibana feature privilege deprecations. Use when deprecating features, renaming features, splitting features, consolidating features, moving privilege capabilities, reviewing deprecation PRs, or working with the replacedBy mapping system.
Files:
- .agents/skills/kibana-privilege-deprecation/SKILL.md
- .agents/skills/kibana-privilege-deprecation/references/reference.md

## optimize-bundle-size
Description: Reduce plugin `page load bundle size` and avoid unnecessary increases in `packages/kbn-optimizer/limits.yml`. Use when proactively optimizing bundles, investigating CI page-load overages, or reviewing PRs that change bundle limits.
Files:
- .agents/skills/optimize-bundle-size/SKILL.md

## scout-api-testing
Description: Use when creating, updating, debugging, or reviewing Scout API tests in Kibana (apiTest/apiClient/requestAuth/samlAuth/apiServices), including auth choices, response assertions, and API service patterns.
Files:
- .agents/skills/scout-api-testing/SKILL.md
- .agents/skills/scout-api-testing/references/scout-api-auth.md
- .agents/skills/scout-api-testing/references/scout-api-services.md

## scout-best-practices-reviewer
Description: Review Scout UI/API tests (including Scout test migrations) for best practices, reuse, and parity.
Files:
- .agents/skills/scout-best-practices-reviewer/SKILL.md

## scout-create-scaffold
Description: Generate or repair a Scout test scaffold for a Kibana plugin/package (test/scout*/{api,ui} Playwright configs, fixtures, example specs). Use when you need the initial Scout directory structure; prefer `node scripts/scout.js generate` with flags for non-interactive/LLM execution.
Files:
- .agents/skills/scout-create-scaffold/SKILL.md

## scout-migrate-from-ftr
Description: Use when migrating Kibana Functional Test Runner (FTR) tests to Scout, including decisions about UI vs API tests, mapping FTR services/page objects/hooks to Scout fixtures, and splitting loadTestFile patterns.
Files:
- .agents/skills/scout-migrate-from-ftr/SKILL.md

## scout-migration-planner
Description: Analyze an FTR test directory and produce a structured Markdown migration plan for Scout. Use when planning an FTR-to-Scout migration, triaging FTR suites for Scout readiness, or when asked to create a migration plan before writing code. Does not write test code; outputs an architectural blueprint for an executor skill or human.
Files:
- .agents/skills/scout-migration-planner/SKILL.md
- .agents/skills/scout-migration-planner/references/output_template.md

## scout-ui-testing
Description: Use when creating, updating, debugging, or reviewing Scout UI tests in Kibana (Playwright + Scout fixtures), including page objects, browser authentication, parallel UI tests (spaceTest/scoutSpace), a11y checks, and flake control.
Files:
- .agents/skills/scout-ui-testing/SKILL.md
- .agents/skills/scout-ui-testing/references/scout-browser-auth.md
- .agents/skills/scout-ui-testing/references/scout-ui-parallelism.md

## validate-oas
Description: Use when you need a quick VALID or NOT VALID result for a scoped Kibana OAS area, and first ensure the generated `oas_docs` inputs are up to date so validation runs against the current environment rather than stale snapshots.
Files:
- .agents/skills/validate-oas/SKILL.md

## Flat File List
- .agents/skills/api-authz/SKILL.md
- .agents/skills/branch-readiness-checks/SKILL.md
- .agents/skills/buildkite-logs/SKILL.md
- .agents/skills/codeql/SKILL.md
- .agents/skills/cypress-to-scout-migration/SKILL.md
- .agents/skills/cypress-to-scout-migration/references/cypress-vs-scout-differences.md
- .agents/skills/cypress-to-scout-migration/references/example-migration.md
- .agents/skills/cypress-to-scout-migration/references/flakiness-risk-patterns.md
- .agents/skills/cypress-to-scout-migration/references/migration-best-practices.md
- .agents/skills/debug-oas/SKILL.md
- .agents/skills/encrypted-saved-objects/SKILL.md
- .agents/skills/enzyme-to-rtl/SKILL.md
- .agents/skills/evals-create-suite/SKILL.md
- .agents/skills/evals-write-spec/SKILL.md
- .agents/skills/evals-write-spec/references/evaluator-patterns.md
- .agents/skills/fix-package-docs/SKILL.md
- .agents/skills/ftr-testing/SKILL.md
- .agents/skills/gh-create-issue/SKILL.md
- .agents/skills/gh-enhance-issue/SKILL.md
- .agents/skills/kibana-api/SKILL.md
- .agents/skills/kibana-privilege-deprecation/SKILL.md
- .agents/skills/kibana-privilege-deprecation/references/reference.md
- .agents/skills/optimize-bundle-size/SKILL.md
- .agents/skills/scout-api-testing/SKILL.md
- .agents/skills/scout-api-testing/references/scout-api-auth.md
- .agents/skills/scout-api-testing/references/scout-api-services.md
- .agents/skills/scout-best-practices-reviewer/SKILL.md
- .agents/skills/scout-create-scaffold/SKILL.md
- .agents/skills/scout-migrate-from-ftr/SKILL.md
- .agents/skills/scout-migration-planner/SKILL.md
- .agents/skills/scout-migration-planner/references/output_template.md
- .agents/skills/scout-ui-testing/SKILL.md
- .agents/skills/scout-ui-testing/references/scout-browser-auth.md
- .agents/skills/scout-ui-testing/references/scout-ui-parallelism.md
- .agents/skills/validate-oas/SKILL.md
