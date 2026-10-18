# Repository Agent Contract

## File size

- Keep every source file at or below 500 LOC. Tests, docs and CSS are exempt. Markdown is documentation, not source. Split a source file before completion if your change takes it over the limit.
- Hooks activate automatically on managed development accounts and new Codex environments. Pre-commit checks only staged authored text: at most 5,000 tokens (bytes / 4). See [.githooks/README.md](.githooks/README.md) for generated-file exemptions and splitting instructions.
