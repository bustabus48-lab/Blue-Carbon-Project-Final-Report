# Report Execution Pack for Codex

## 1. Objective
Use Codex as a supervised multi-agent writing environment to produce the Final Report as a synthesis of all approved source reports and technical outputs.

## 2. Whether GitHub is needed
For Codex cloud tasks, GitHub-backed repositories are the standard setup: OpenAI’s help guidance says Codex currently supports GitHub (cloud-hosted) as its source code management system, while the product materials describe tasks running in cloud sandboxes preloaded with a repository. citeturn138170search2turn138170search0

## 3. Best-fit project model
Treat the report as a repo-managed document production project, not as one long prompt.

### Roles
- **Lead editor**: owns narrative, scope, and approvals
- **Extractor agent**: reads source reports into templates
- **Synthesis agent**: builds matrices and cross-report findings
- **Drafting agent**: drafts chapters against outline
- **Authoring agent**: turns drafted material into audience-ready prose for policy makers, academics, and development partners while preserving evidence-backed findings and avoiding fact invention
- **QA agent**: checks consistency, evidence traceability, and duplication

## 4. Execution sequence

### Phase A: Repo setup
1. Create a GitHub repo for the report project
2. Upload all source documents into `source_reports/`
3. Add this workflow pack and `AGENTS.md`
4. Confirm file naming conventions
5. Create a decision log in `notes/decision_log.md`
6. Confirm the three standalone source reports required for final authoring are present in markdown:
   - National MRV Report
   - Drone Survey / EOSDA Report
   - Carbon Inventory Report

### Phase B: Structured extraction
For each report, create a markdown extraction note using `templates/source_extraction_template.md`.

Priority requirement before integrated drafting:
- the National MRV Report, Drone Survey / EOSDA Report, and Carbon Inventory Report should each exist as standalone `.md` source reports so they can be extracted directly.

Outputs:
- one extraction file per report
- issue log of unclear or contradictory data
- list of reusable tables/figures from source reports

### Phase C: Synthesis
Populate:
- `templates/synthesis_matrix.csv`
- `templates/site_profile_template.md`
- `templates/findings_traceability_table.csv`

Goal:
Translate report-by-report findings into site-level and cross-cutting insights.

### Phase D: Drafting
Draft in this order:
1. Introduction and scope
2. Methods overview
3. Study area context
4. Integrated baseline findings
5. Cross-cutting synthesis
6. Drone survey, EOSDA, and monitoring readiness
7. MRV system
8. Restoration and management implications
9. Recommendations and next steps
10. Conclusion
11. Executive summary last

### Phase E: Authoring layer
After chapter drafting, run a dedicated authoring pass to convert technical material into decision-oriented report prose.

Outputs:
- final-report-ready chapter text for policy and management audiences
- standalone National MRV, Drone Survey / EOSDA, and Carbon Inventory reports in markdown where those deliverables are part of the reporting package
- flagged list of missing implementation inputs, especially for EOSDA account setup, uploaded areas of interest, screenshots, and monitoring workflow evidence

Rules:
- do not add new findings during the authoring pass
- define acronyms on first use
- keep methods short in the main report and move detail to annexes
- distinguish clearly between completed evidence, pending inputs, and recommendations

### Phase F: QA
Run checks for:
- conflicting figures
- inconsistent site names
- unsupported recommendations
- duplicate text across chapters
- unfilled placeholders
- missing annex references

## 5. Chapter logic
The final report should answer these questions:
1. What is the current state of mangroves in the study areas?
2. What are the main ecological and socio-economic pressures?
3. What is the carbon significance of the mangrove landscapes?
4. Which areas should be prioritized for protection, restoration, and monitoring?
5. How will drone, EOSDA, and MRV systems sustain ongoing monitoring?

For users who also need a separate Drone Survey report, the companion report should answer:
1. Which areas of interest, plots, or monitoring polygons are already evidenced in the repository?
2. Which drone-linked outputs are available now, and which report-ready assets are still missing?
3. What must be completed before continuous monitoring in EOSDA Crop Monitoring can be reported as operational?

## 6. Prompting strategy for Codex
Do not ask for the entire 100-page report in one task.
Use bounded prompts:
- one task per source extraction
- one task to prepare or refine each required standalone `.md` source report before extraction begins
- one task for matrix population
- one task per chapter
- one QA pass per chapter
- one final harmonization pass

## 7. Human checkpoints
Pause for human approval after:
- report outline
- all extraction notes
- synthesis matrix
- first draft of integrated findings chapter
- first draft of recommendations
- final QA report

## 8. Deliverables from the workflow
- structured extraction notes
- synthesis matrix
- site profiles
- chapter drafts
- authoring-layer outputs for the Final Report and the standalone MRV, Drone Survey / EOSDA, and Carbon Inventory reports where required
- figure and table inventory
- findings traceability table
- final editorial checklist

## 9. Minimum inputs before final authoring pass
Do not finalize the report package until the following are either available or explicitly marked as pending:
- approved blueprint and source reports
- completed National MRV Report in markdown
- completed Drone Survey / EOSDA Report in markdown
- completed Carbon Inventory Report in markdown
- resolved or logged contradictions from extraction and synthesis stages
- confirmed list of drone survey areas of interest and boundary files
- EOSDA account setup status, uploaded AOIs/polygons, and any screenshots or access notes intended for reporting
- any monitoring workflow evidence needed to support claims about continuous monitoring

## 10. Definition of done
The report is ready for final editorial packaging when:
- all chapters are drafted
- all major claims are traceable
- placeholders are resolved or clearly marked
- recommendations are evidence-linked
- figures and tables are numbered and referenced
- terminology is consistent
- duplication is minimized
