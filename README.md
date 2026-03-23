# Blue Carbon Final Report Project

This repository is a controlled writing environment for producing the **Final Report** for the Blue Carbon Assessment Consultancy.

## Purpose
The final report will synthesize:
- Mangrove Geospatial Extent Report
- Socio-Economic Report
- Ecosystem Health Report
- Carbon Inventory Report
- Drone Survey plots and outputs
- EOSDA hosting and monitoring setup
- MRV system documentation

It can also support a **companion Drone Survey / EOSDA monitoring report** when the project needs a standalone, implementation-focused output alongside the main Final Report.

## Recommended workflow
1. Place all source reports in `source_reports/`
2. Use the prompts in `prompts/` to extract structured notes from each source
3. Build the synthesis matrix in `templates/synthesis_matrix.csv`
4. Draft report chapters in `drafts/`
5. Run an authoring pass to convert technical draft material into readable report prose for policy makers, academics, and development partners
6. Run the QA checklist in `qa/QA_CHECKLIST.md`
7. Consolidate into the final manuscript and any companion Drone Survey report

## Folder structure
- `source_reports/` original reports and source material
- `templates/` structured extraction and synthesis templates
- `prompts/` reusable agent prompts for Codex
- `workflows/` end-to-end instructions and execution sequence
- `drafts/` chapter drafts
- `annex/` figure, table, and annex support files
- `qa/` consistency and editorial checks
- `notes/` working notes, issue logs, decision logs

## Files to upload first
- Contract agreement
- Negotiation minutes / payment schedule
- Terms of Reference
- Inception report
- Geospatial extent report
- Socio-economic report
- Ecosystem health report
- Carbon inventory report
- Drone survey outputs
- EOSDA screenshots / notes
- MRV documentation / data dictionary / screenshots

## Suggested branch strategy
- `main` = approved material only
- `draft/core-structure`
- `draft/extractions`
- `draft/synthesis`
- `draft/chapter-writing`
- `review/final-qa`

## Core rule
This repo is for **evidence-led synthesis**. The final report must not be a stitched set of summaries. Every major claim should be traceable to one or more source reports.
