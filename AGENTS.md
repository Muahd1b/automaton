# Automaton Agent Contract

## Boundaries
- Preserve the sovereign agent runtime, state, wallet, and package boundaries.
- Read only task-relevant README or package documentation.
- Domain routing: read [domain.md](docs/agents/domain.md).

## Validation
- Default: `pnpm vitest run <test-file>` for one affected test file; use package-scoped TypeScript checks when available.
- `pnpm test`, `pnpm build`, recursive workspace builds, and complete test suites are broad and run only after an explicit user request.

## File size

- Keep every source file at or below 500 LOC. Tests, docs and CSS are exempt. Markdown is documentation, not source. Split a source file before completion if your change takes it over the limit.
- Hooks activate automatically on managed development accounts and new Codex environments. Pre-commit checks only staged authored text: at most 5,000 tokens (bytes / 4). See [.githooks/README.md](.githooks/README.md) for generated-file exemptions and splitting instructions.
