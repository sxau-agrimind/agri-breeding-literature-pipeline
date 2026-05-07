# Versioning

## Current Version

The current public lab release is `v0.1.0`, released on 2026-04-21.

This is the initial public release of the codebase and workflow for multi-source agricultural breeding literature retrieval, preprocessing, relevance filtering, `retrieval_word` tagging, cleaning, deduplication, and raw inventory reporting.

## Versioning Policy

This repository follows semantic versioning in spirit:

- Patch updates may clarify documentation, fix small bugs, or improve validation checks.
- Minor updates may add source-layer improvements, filtering refinements, tests, or packaging support.
- Major updates would be reserved for substantial workflow or public-interface changes.

The repository is a research engineering codebase rather than a fully productized package, so version numbers describe the public codebase and workflow state rather than a packaged library release.

## Release Scope

Versioned release content includes:

- Source code under `src/`
- Entry scripts under `scripts/`
- Configuration templates under `configs/`
- Public documentation under `docs/`
- CI workflow files
- Citation and repository metadata

Versioned release content does not include:

- Full raw dumps
- Generated JSONL corpus files
- Full cleaned corpora
- Private datasets
- Local caches or machine-specific runtime outputs

## Current Public Status

`v0.1.0` should be understood as an initial lab release of a configurable workflow. It supports PubMed, arXiv, bioRxiv, medRxiv, and chemRxiv, but source availability, network conditions, local dump availability, and configuration choices still affect runtime behavior.

xRxiv relevance filtering remains under iterative refinement. bioRxiv uses a relaxed source-specific filtering policy, while medRxiv and chemRxiv use stricter policies because their candidate retrieval results are noisier for agricultural breeding use cases.

## Future Directions

Potential future versions may include:

- Improved xRxiv relevance filtering
- More systematic tests for cleaning, reporting, and source-layer behavior
- Packaging improvements
- Expanded documentation
- Optional Docker support if a Docker workflow is implemented later
