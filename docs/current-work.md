# Current work

## Current focus and status

The current milestone is the public documentation baseline defined in [PROJECT.md](../PROJECT.md). It contains the reviewed README and architecture proposal, three explanatory figures and editable diagram sources.

The source documents completed a seven-step editorial cycle. The [evidence summary](../evidence/README.md#editorial-review) states what that review covered and the limits of the public copy. No router, classifier evaluation or conversation-cost experiment has been implemented or run.

## Next actions

The proposed next milestone is a small evidence/applicability catalog and [coverage/economics audit](proposal.md#1-audit-feasibility), followed by classifier validation if there is a useful opportunity. It requires owner choices about workload, exact configurations, mappings and acceptance; commissioning that work is a separate decision.

Provider integration and full conversation trials depend on those findings. See the [design contract](design.md#implementation-contract) before beginning implementation.

## Findings and handover

Published benchmark qualification is not a per-request success guarantee. The selector minimizes one next-call forecast, while the intended benefit is evaluated over complete conversations. Cheap reliable classification and useful evidence transfer remain hypotheses.

Publication checks and their limits are discoverable through [checks](../tests/README.md), [evidence](../evidence/README.md) and the repository's Git history. Keep status and consequential findings current without importing a duplicate private activity log.
