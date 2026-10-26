---
name: asd-single-paper-classification-workflow
description: Classify one paper for the Autonomous Scientific Discovery / Agent for Science review, including evidence-based inclusion, multi-module scientific-object classification, note filing, and owner-data writeback. Use when adding or reclassifying an individual paper; not for broad searches or full-library audits.
metadata:
  short-description: Classify one ASD paper end to end
---

# ASD Single-Paper Classification Workflow

Use this skill when a person needs to add, review, or correct a single paper in the `Autonomous Scientific Discovery` project. The desired result is a traceable inclusion decision and scientific-object classification, not merely a plausible label.

## Project Discovery

Locate the project root named `Autonomous Scientific Discovery`. Do not assume the current working directory is the project root. Before changing a paper record, read:

- `review_scope_and_classification_policy.md`
- `domain_classification_rules.md`
- `science_domain_taxonomy.md`
- `Data/classification_code_index.json`
- `Data/field_ownership_matrix.md`
- `Paper_Lists/agent_master_paper_list.md`
- `paper_note_templates_and_prompts/ASD_annotation_schema.md`

For a paper that will enter or change the core library, also read the note template, the per-module mapping ledger, and the discipline-code policy listed in [project-layout-and-writeback.md](references/project-layout-and-writeback.md).

## Non-Negotiable Rules

1. Include only Agent-for-Science papers. A core paper must have all of: a clear scientific goal, multi-step action, at least one Agent capability, and an explicit research-workflow role.
2. Closed-loop or full autonomous discovery is not a core inclusion requirement. Record it as evidence of autonomy rather than using it as an inclusion gate.
3. Classify by the concrete scientific object and evidence, never by venue, author affiliation, model type, or Agent architecture.
4. Use first-hand sources for a classification decision: full text/PDF first, then official preprint or publisher page, followed by official project, benchmark, or supplement. Existing notes and legacy classes are leads only.
5. Record every supported `01`-`11` module when the paper reports object-specific experiments, validations, benchmark tasks, case studies, or results. A module need not be the paper's main contribution.
6. Use the independent `01.04` bucket only when no concrete scientific-object evidence supports any `01`-`11` module. `01.04` never appears inside `scientific_object_modules`.
7. When evidence is weak, inaccessible, or conflicts materially, preserve the uncertainty as `needs_review` or `source_limited`; do not force a definitive classification.

## Classification Procedure

### 1. Establish identity and evidence

- Search the master list and `Data/papers.jsonl` by title, DOI, arXiv identifier, and normalized author/year before creating a record. Merge a version into the existing `ASD-xxxx` record instead of creating a duplicate.
- Gather canonical title, authors, year, venue, DOI/URL, and the best available first-hand sources.
- Extract short, attributable evidence for four Agent gates, the research object(s), the workflow, and the validation/result(s). Keep locations such as page, section, figure, table, official abstract, or URL.

### 2. Decide the record status

Apply the four Agent gates together:

| Decision | Use when |
|---|---|
| `to_read` / `included` | All four gates are supported and classification evidence is sufficient for a core record. |
| `candidate` | A likely in-scope paper needs evidence before inclusion. |
| `needs_review` | Evidence, boundary, identity, or source access is genuinely unresolved. State what would resolve it. |
| `background_only` | Useful review, roadmap, benchmark, infrastructure, or context paper that does not function as an included Agent-system study. |
| `excluded` | Clearly fails one or more Agent gates, is out of scope, or is a duplicate. Preserve the reason. |

Do not exclude a paper merely because it is a benchmark, a simulation study, or lacks a robot/wet-lab loop. Do exclude an ordinary prediction model, one-shot assistant, or automation system that lacks Agent behavior and a research-workflow role.

### 3. Assign scientific-object modules

For each candidate module, write an evidence row before assigning it:

| Module | Concrete object | Experiment, validation, task, case, or result | Source location | Confidence |
|---|---|---|---|---|

Apply these rules in order:

1. If one or more rows support concrete objects, assign all corresponding `01`-`11` modules and set `single_module` or `multi_module`.
2. If no row supports a concrete object but the work is an in-scope general research Agent, use `general_method_without_concrete_object_experiments` and `01.04_general_asd_methods_without_concrete_object_experiments`.
3. Select `primary_module_for_filing` only to decide the note/PDF directory. It does not erase other supported modules.
4. Apply the taxonomy's fixed secondary tree for `03`, `04`, `06`, and `07`. For `06` and `07`, assign a supported tertiary code when evidence permits. Do not invent a finer code from the title alone.
5. Resolve adjacent boundaries from `domain_classification_rules.md`, especially `03/04`, `05/10`, `06/07`, `01.04/concrete modules`, and `01.04/11.07`.

### 4. Produce the classification record

Before any writeback, provide a concise decision record with:

- canonical identity and source trail
- status and four Agent-gate evidence
- supported module(s), coverage mode, and `01.04` decision
- per-module object-evidence rows
- primary filing module and secondary/tertiary codes where supported
- boundary reasoning, confidence, source limitations, and next action

If the decision is a core record, draft or update the structured note using the project template. A complete note contains an Evidence Log and explicitly explains inclusion, scientific-object modules, workflow role, methods, validation, limitations, and review value.

## Writeback and File Management

Follow the ownership and ordering rules in [project-layout-and-writeback.md](references/project-layout-and-writeback.md). In particular:

- Edit owner facts before generated data.
- Update the master record and module-specific taxonomy mappings for a confirmed classification.
- Add or update a stable discipline-local code only when the filing position is clear; never re-rank or reuse existing codes.
- Put a core note under the directory for `primary_module_for_filing`, using `FirstAuthor_Year_ShortTitle.md`. Note location is not classification evidence.
- Store or link primary sources/PDFs only when the task authorizes that action; do not infer PDF status from a blank or nonblank path.
- Do not hand-edit derived exports such as `Data/papers.jsonl`, `Data/papers.sqlite`, manifests, registries, or CSV snapshots.

After owner edits, run the canonical project pipeline:

```powershell
python 'Autonomous Scientific Discovery/scripts/run_structured_data_pipeline.py'
```

Resolve `ERROR` findings before considering the paper classification complete. Preserve `WARNING` findings in the record or review queue.

## Handoff Standard

Report the changed paper ID, status, modules/bucket, filing module, evidence sources checked, files changed, pipeline result, and any unresolved question. For classification-sensitive changes, state why nearby classes were not selected.

Use the project's controlled English status values and codes, while writing explanatory prose in Chinese unless the task requires otherwise.
