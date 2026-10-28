# Tests and assessments

## Documentation publication checks

For the initial documentation milestone, check the following:

1. **Inventory:** the public tree contains the intended README, proposal, figures, editable diagram sources and supporting project records. No private working history or temporary runtime is staged.
2. **Source fidelity:** preserve the current README's purpose, rationale and five examples and the current proposal's architecture, numerical examples, code and evidence limits. Publication changes are document paths, project navigation and supporting project records.
3. **Navigation and presentation:** every local Markdown link and heading fragment resolves; all three images are present and match the selected source assets; diagrams remain legible. Inspect the HTML sources and proposal in suitable viewers.
4. **Public-content scope:** inspect the full staged text and metadata for credentials, personal machine paths, private chat links and unintended personal information. Use only the existing configured Git attribution.
5. **Publication:** after pushing, verify the remote commit and tree against the checked local commit, confirm public visibility and anonymous repository access, and confirm a clean synchronized working tree.

Useful Git inspections before committing include `git diff --cached --check`, `git diff --cached --stat`, `git diff --cached` and `git ls-files`. Record what actually ran and distinguish prepared checks from verified results. A pattern scan alone is not proof that sensitive content is absent.

## Router evaluation remains planned

There is no executable router or software test suite in this baseline. The [proposal's evaluation plan](../docs/proposal.md#evaluation-and-acceptance) separates evidence/economics feasibility, held-out classifier and selector validation, diagnostic replay, and complete-conversation comparisons. These activities need their own commissioned scope, implementation contract and retained results before any outcome claim.

Connect future checks to the [project agreement](../PROJECT.md), [design](../docs/design.md#implementation-contract) and [evidence](../evidence/README.md). A documentation check is not evidence that the router works.
