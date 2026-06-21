# Contributing

Contributions are welcome. Please read this guide before opening a pull request.

## What belongs in this list

This registry is for resources that provide vector storage, indexing, or similarity search for AI and RAG applications. Acceptable entries include:

- Vector databases (managed, self-hosted, or embedded).
- Vector search libraries and indexing algorithms.
- Multi-model databases where vector search is a first-class, documented capability.
- Benchmarks, evaluation datasets, and leaderboards for vector retrieval.
- Search engines that natively combine vector similarity with keyword/filtered search.

## What does **not** belong

- General SQL or NoSQL databases without a documented vector-search extension or feature.
- Embedding model providers that do not include a storage or retrieval system.
- Closed-source or paywalled-only tools with no public documentation.
- Duplicate entries.

## Quality bar

Every submission must be:

1. **Publicly accessible** — open source or publicly documented.
2. **Actively maintained** — last meaningful commit or release within the last 12 months (exceptions for widely adopted reference projects).
3. **Documented** — a real README or docs page with setup or install instructions.
4. **Correctly categorized** — placed under the category that best matches its deployment model and primary capability.
5. **Honestly labeled** — use the `Official` or `Community` badge.

## Entry format

Use this pattern:

```markdown
- **[Name](URL)** `Official` — One-sentence description.
  - Install: `command here`
```

If there is no install command, omit the install line.

## Category sections

The README is organized by **capability and deployment model**. New category sections are allowed only if they contain at least five entries.

## Pull request process

1. Fork the repository.
2. Add your entry in the correct category section.
3. Run `./scripts/validate-links.sh` and fix any broken links or anchors.
4. Open a pull request with a clear description of the resource and why it fits.

One resource per pull request is preferred.
