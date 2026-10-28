# Design and approach

## Approach and important parts

The [architecture proposal](proposal.md) is the single detailed design source. It describes a classifier for the latest request's required abilities, reviewed published evidence, deterministic model selection, provider execution and cost records in one service.

The design is a proposal. It has not been implemented or shown to deliver savings. Begin with the [feasibility audit](proposal.md#1-audit-feasibility), then validate classification before committing to provider integration and conversation trials.

## Connections and open questions

The [project agreement](../PROJECT.md) distinguishes documentation acceptance from the intended cost and quality outcome. The [proposal's decision table](proposal.md#decisions-before-implementation) retains the unresolved workload, evidence, classifier, execution and acceptance choices.

The [figures](assets/diagrams/01-routing-overview.png), [editable sources](../src/README.md), [checks](../tests/README.md) and [evidence limits](../evidence/README.md) support assessment. The illustrations use hypothetical examples; they are not model-performance results.

## Implementation contract

For this documentation publication, the required checks are the [documentation publication checks](../tests/README.md#documentation-publication-checks): deliberate file inventory, source fidelity, working links/assets, public-content inspection and matching local/remote Git state.

Before router implementation, agree on the relevant proposal decisions and prepare checks covering the intended behavior, interactions, evidence limits and acceptance conditions. This documentation milestone supplies no executable router contract or implementation approval. The staged [evaluation plan](proposal.md#evaluation-and-acceptance) identifies the later questions and evidence needed.

## Findings and changes

Retain important reasons in [decisions](decisions.md) and update [current work](current-work.md) as findings change the approach. Keep one current design source rather than competing copies of the proposal.
