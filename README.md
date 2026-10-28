# Capability Based Model Routing

## Purpose

Explore whether choosing a language model for each conversation turn can reduce total cost while maintaining answer quality within an agreed range. The choice uses the abilities required by the latest request, published model measurements and explicit selection rules.

## Rationale

The idea is to use existing, reasonably reliable measurements of model abilities as the basis for choosing the best model for each conversation turn. A classifier identifies which abilities the latest request requires, using the conversation history for context. Selection rules then match those requirements to the published measurements and choose a model under the application's quality and cost requirements.

The classifier supplies the link between what the user needs and what has been measured about each model. For the policy explored here, the best model is the eligible one with the lowest estimated next-call cost. Published measurements remain imperfect evidence; whether this approach reduces total conversation cost while maintaining quality must be validated across complete conversations.

## Overview

1. **Reuse published measurements of model abilities.** Build model profiles from reviewed existing benchmarks for exact model configurations, preserving the scope and limitations of each measurement.

   *Example: Use published results from AIME for competition mathematics, LiveCodeBench for its evaluated programming scenarios, and IFEval for following verifiable explicit instructions.*

2. **Identify the abilities required by the latest request.** A classifier uses the full supported conversation history for context and can assign several ability labels. Low cost and reliable classification are goals to validate.

   *Example: After a conversation about travel, “calculate how to split these expenses” requires mathematics and understanding the earlier information. The classifier labels this latest request, using the history to identify the expenses.*

3. **Choose a model using explicit rules.** Select the available model with the lowest estimated next-call cost that meets every applicable benchmark requirement and operational constraint. Use explicit exception or unavailable outcomes when qualification fails.

   *Example: If two models meet the relevant mathematics and instruction-compliance thresholds and both support the conversation, choose the one with the lower estimated call cost.*

4. **Reconsider the selection at every user turn.** The appropriate model can change as the conversation moves between different kinds of work. Keep the selected configuration through that turn's tool loop: the sequence of model calls, tool calls and returned results within the turn.

   *Example: A request to draft an email and a later request to calculate interest can go to different models.*

5. **Check whether routing delivers actual savings.** Evaluate quality and total cost across complete conversations, including classification, caching, retries, repairs and additional work.

   *Example: Compare routed conversations against both strong and economical fixed-model baselines to see whether total spending falls while quality stays within an agreed acceptable range.*

This workspace contains research and a proposed architecture. Cost savings and maintained quality remain hypotheses to validate.

See the [architecture proposal](docs/proposal.md) for the design, diagrams, evidence policy and evaluation plan.

## Project records

- [Project agreement](PROJECT.md): scope, expectations and open decisions.
- [Design](docs/design.md) and [architecture proposal](docs/proposal.md): the approach and detailed design.
- [Current work](docs/current-work.md) and [decisions](docs/decisions.md): status, reasons and next steps.
- [Checks](tests/README.md) and [evidence](evidence/README.md): what has been assessed and what remains unproven.
- [Diagram sources](src/README.md) and [delivery](docs/delivery.md): editing and using the documentation.

## Versions and releases

Changes are recorded in [CHANGELOG.md](CHANGELOG.md) under **Unreleased** until a release is prepared. This repository starts its own release history; no version tag has been created.

Use `MAJOR.MINOR.PATCH` for releases: major for incompatible changes, minor for compatible additions, and patch for corrections that preserve intended behavior and agreements. A release needs a reviewed dated changelog entry and an annotated tag on its exact commit. Published tags remain fixed; later corrections use a new version.
