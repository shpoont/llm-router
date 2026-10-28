# Decisions

## 2026-10-28 — Publish a documentation baseline

**Status: agreed direction.** The repository owner requested a public repository named `llm-router`, following Project Structure, with the README, proposal and assets committed.

Use the current README and proposal as the content sources. Put the detailed proposal in [docs/proposal.md](proposal.md), public figures in `docs/assets/diagrams/`, and editable HTML in `src/diagrams/`. The design entry point links to the proposal rather than duplicating it. Keep project records proportionate to the documentation stage.

This publication does not adopt the proposed architecture as a production implementation or establish the cost/quality outcome. Private conversations, local review packets and transient tooling remain outside this baseline. The public [evidence summary](../evidence/README.md) retains the relevant review conclusions and limitations.

## Unresolved design choices

The [proposal's decisions before implementation](proposal.md#decisions-before-implementation) remain proposed parameters for adoption. In particular, exception reasons, classifier context envelope, evidence mappings, exact model configurations and acceptance thresholds are not silently selected by publishing the document.

## Release history

Use a new project release history and the [README release convention](../README.md#versions-and-releases). This initial publication is recorded under Unreleased; creating a public repository and initial commit does not create a tagged release.
