# Blue Carbon Final Report Project

This repository is a controlled writing environment for producing the **Final Report** for the Blue Carbon Assessment Consultancy.

## Purpose
This repo produces the **Blue Carbon Final Report**, which is one of four coordinated deliverables for the assignment. The full deliverable set is:

| # | Report | Author | Status |
|---|---|---|---|
| 1 | **Blue Carbon Final Report** (this repo) | Ecological Nest / Team Leader | In progress |
| 2 | **MRV System Report** (standalone) | Team Leader | To be authored separately |
| 3 | **Drone Survey and EOSDA Continuous Monitoring Report** (standalone) | Team Leader | To be authored separately |
| 4 | **Carbon Inventory Report** (standalone) | Carbon Team | Pending delivery |

The Final Report synthesizes and cross-references the three companion reports. It does not replicate their content at the same level of detail. Chapters 8 and 9 of the Final Report provide summary treatments and direct cross-references to the standalone Drone/EOSDA and MRV reports respectively.

## Recommended workflow
1. Place all source reports in `source_reports/`
2. Use the prompts in `prompts/` to extract structured notes from each source
3. Build the synthesis matrix in `templates/synthesis_matrix.csv`
4. Draft report chapters in `outputs/drafts/`
5. Run the QA checklist in `qa/QA_CHECKLIST.md`
6. Consolidate into the final manuscript

## Folder structure
- `source_reports/` original reports and source material
- `templates/` structured extraction and synthesis templates
- `prompts/` reusable agent prompts for Codex
- `workflows/` end-to-end instructions and execution sequence
- `outputs/drafts/` chapter drafts
- `outputs/figures/` figures, maps, diagrams, screenshots
- `outputs/tables/` final tables
- `outputs/annexes/` annex drafts and supporting material
- `qa/` consistency and editorial checks
- `notes/` working notes, issue logs, decision logs

## Files to upload / provide
**For the Final Report (this repo):**
- Contract agreement
- Negotiation minutes / payment schedule
- Terms of Reference
- Inception report ✓
- Geospatial extent report
- Socio-economic report
- Ecosystem health report ✓
- Carbon inventory report — *from Carbon Team*

**For the standalone Drone Survey + EOSDA Report (from Team Leader):**
- Drone orthomosaics and flight mission logs
- EOSDA area-of-interest setup and hosting screenshots
- Condition-mapping panels and coverage maps

**For the standalone MRV System Report (from Team Leader):**
- MRV system architecture documentation
- Dashboard and visual exports from `GAB-Climate-Smart/blue-carbon-mrv`
- Data dictionary and data flow diagrams

## Suggested branch strategy
- `main` = approved material only
- `draft/core-structure`
- `draft/extractions`
- `draft/synthesis`
- `draft/chapter-writing`
- `review/final-qa`

## Core rule
This repo is for **evidence-led synthesis**. The final report must not be a stitched set of summaries. Every major claim should be traceable to one or more source reports.
