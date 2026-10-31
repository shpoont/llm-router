# Current project agreement

## Purpose and intended result

Investigate capability based model routing as described in the [README](README.md). The intended benefit is lower total conversation cost while maintaining an agreed level of answer quality. That benefit is a hypothesis, not an achieved result.

The current deliverable is a public documentation baseline containing the README, architecture proposal and its three diagrams, with enough context to assess and continue the work.

## Scope and expectations

- **Delivery acceptance:** the requested documents and editable diagram assets are present, their local links work, and the public commit contains only the intended material.
- **Outcome success:** routing must eventually demonstrate acceptable quality and useful conversation-level savings against credible strong and economical fixed-model baselines. No such result is established here.
- **Execution constraints:** this baseline is documentation only. It does not authorize implementation, paid model trials, a new solver-profile benchmarking program or publication of private working records.

The documentation milestone ends when the intended commit is publicly available and its contents and repository visibility have been verified. Research and implementation milestones need their own scope and checks. See [checks](tests/README.md), [evidence](evidence/README.md) and [delivery](docs/delivery.md).

## People and responsibilities

The repository owner sets direction and approves the workload, model pool, evidence policy, acceptance criteria and consequential commitments. Contributors prepare and check work within the authorized scope. Specialist evidence review and statistical study responsibilities remain to be assigned when that work is commissioned.

## Assumptions and open questions

The [proposal's decisions before implementation](docs/proposal.md#decisions-before-implementation) remain open. Published evidence must be sufficiently reliable and applicable to the chosen scenarios; the classifier must recover requirements at acceptable cost; conditional model choices must improve complete-conversation economics. No particular classifier, solver pool or threshold has been adopted for production.

## Connected work

Follow [design](docs/design.md), [current work](docs/current-work.md) and [decisions](docs/decisions.md). This repository applies Project Structure's organization and discoverability guidance, adapting its records to the present documentation stage. The adopted starter baseline and upstream source are recorded in [.project-structure.yaml](.project-structure.yaml).
