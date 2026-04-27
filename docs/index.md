# Agri Breeding Literature Pipeline Docs

This documentation describes the public codebase and workflow for multi-source agricultural breeding literature retrieval, preprocessing, cleaning, deduplication, and reporting.

The repository does not include full raw dumps, full cleaned corpora, or private datasets. It is a research engineering codebase intended to make the workflow inspectable and reproducible, not a fully productized turnkey package.

## What This Project Covers

- PubMed and arXiv online retrieval
- bioRxiv, medRxiv, and chemRxiv local dump retrieval
- Source-specific relevance filtering for xRxiv records
- `retrieval_word` tagging for query pair traceability
- Cleaning and deduplication across source outputs
- Raw inventory reporting
- Documentation and CI checks

## Recommended Reading Order

1. [Architecture](architecture.md)
2. [Pipeline Overview](pipeline_overview.md)
3. [Configuration](configuration.md)
4. [Scripts Guide](scripts_guide.md)
5. [Project Structure](project_structure.md)
6. [Developer Notes](developer_notes.md)
7. [Known Limitations](known_limitations.md)
8. [Smoke Test](smoke_test.md)

## Important Boundaries

- Public documentation describes code, configuration, examples, and workflow.
- Runtime outputs under `data/raw/`, `data/cleaned/`, and `data/private/` are local-only and should not be committed.
- Generated reports and manually written documentation serve different purposes.
- The raw inventory report counts raw JSONL records; it is not a final quality assessment of a cleaned corpus.
