# GitHub — Reasoning Effort in Dynamic Environments

> Freshness-aware test-time compute for LLM agents in changing environments

## Project Intro

An LLM agent can improve a decision by thinking longer, but the environment may change while it reasons. This project investigates **when more reasoning is worth its cost and when waiting makes an observation stale**.

Our research question is: **How should an LLM agent allocate reasoning effort when the environment can change during inference?** We plan to compare fixed-compute and difficulty-aware approaches with a freshness-aware policy that can act now, think longer, or refresh its observation before acting. Evaluation will consider decision quality, latency or compute, and performance under different rates of environmental change. The benchmarks and implementation are still being selected.

## How to Navigate this Repo

The repository currently contains this README and the planning pages in `docs/`. Code, tests, and tutorial notebooks have **not** been added yet. Update this section whenever a file or directory is introduced, renamed, or removed.

| Path | What it contains | Status |
|---|---|---|
| `README.md` | Project introduction, navigation, usage, standards, and links | Available |
| `docs/proposal-presentation.md` | Proposal checklist and Notion workspace | Available |
| `docs/paper-presentation.md` | Paper-presentation planning page | Available |
| `docs/midterm-presentation.md` | Midterm checklist and Notion workspace | Available |
| `docs/final-presentation.md` | Final-presentation checklist and code-unit/test inventory | Available |
| `docs/final-report.md` | Final-report working outline | Available |
| `docs/related-works.md` | Paper summaries and annotation links | Available |
| Code, tests, and notebooks | Add paths and descriptions as they are created | Not yet available |

When adding code, list **each runnable code file** here with its purpose, usage, and unit-test link. Keep notebook entries here too, including prerequisites and the order in which to run them.

## How to Export & Use the Code

To obtain the current repository:

```bash
git clone https://github.com/shohinirheasarkar/ReasoningEffortInDynamicEnvironments.git
cd ReasoningEffortInDynamicEnvironments
```

You can also select **Code → Download ZIP** on GitHub. At present there is no runnable code or dependency specification, so there is nothing further to install or execute. When implementation is added, document supported systems, required versions, environment setup, any data-access steps, and exact run/test commands here. Avoid machine-specific paths and keep secrets and restricted datasets out of the repository.

## Tutorial Notebooks

No tutorial notebooks have been added yet. For each future notebook, add a link and explain its learning goal, input requirements, expected outputs, and execution order. Notebooks should guide newcomers; reusable logic belongs in testable code modules rather than only in cells.

## Each Code File

Every new code file must:

- Start with a descriptive header explaining its overview, how to run or import it, inputs/outputs, how it was tested, and links to its unit tests.
- Place descriptive paragraph comments before major, non-obvious code sections explaining their purpose and reasoning.
- Use clear names and self-documenting code where appropriate; comments should explain intent rather than repeat the syntax.
- Be organized, loosely coupled, extensible, and portable across supported systems.
- Have relevant unit tests and validation evidence before the associated pull request is merged.
- Trigger an update to **How to Navigate this Repo** when it is added, moved, or changed in purpose.

Documentation should include a user guide when appropriate. Distribute code through this GitHub repository; keep setup instructions and dependencies current so another person can reproduce the work.

## Progress Trackers

- [GitHub Issues](https://github.com/shohinirheasarkar/ReasoningEffortInDynamicEnvironments/issues): concrete tasks, assignments, discussions, and bugs.
- [Pull Requests](https://github.com/shohinirheasarkar/ReasoningEffortInDynamicEnvironments/pulls): code changes, review, and linked tests.
- [GitHub Projects](https://github.com/shohinirheasarkar/ReasoningEffortInDynamicEnvironments/projects): team board; link the specific Project here when it is created.

Suggested workflow: create an Issue → assign an owner → work on a branch → open a PR with `Closes #issue-number` → review tests and documentation → merge and mark complete.

## Links to Major Docs & Presentations

| Deliverable | GitHub planning page | External workspace |
|---|---|---|
| Proposal presentation | [Proposal](docs/proposal-presentation.md) | [Notion Proposal](https://app.notion.com/p/Proposal-3db51fd1aa49800bb589daab142cfb20?pvs=21) |
| Paper presentation | [Paper](docs/paper-presentation.md) | Add link when available |
| Midterm presentation | [Midterm](docs/midterm-presentation.md) | [Notion Midterm](https://app.notion.com/p/Midterm-3db51fd1aa498080ababf65a88bf05d3?pvs=21) |
| Final presentation | [Final](docs/final-presentation.md) | [Notion Final Pres](https://app.notion.com/p/Final-Pres-3db51fd1aa49808eb6e8f13ea4973623?pvs=21) |
| Final report | [Final Report](docs/final-report.md) | Add submission link when available |

The GitHub pages are planning/checklist documents; the Notion links lead to their corresponding external workspaces. Add finished slides and reports to their pages when available.

## Related Works

Use [Related Works](docs/related-works.md) to track each paper by **paper name, summary, and annotated paper or notes**. Include a citation or original-paper link and explain how the paper informs a baseline, assumption, or design choice. Entries will be added as the literature review progresses.

## Team

| Member | Role |
|---|---|
| Pranav Panicker | Project member |
| Shohini Rhea Sarkar | Project member |
| Akash Wudali | Project member |
