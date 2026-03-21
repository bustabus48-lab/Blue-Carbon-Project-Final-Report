# Project Scope Logic

This file exists to prevent agent confusion about why different sites appear in different parts of the report, and to clarify the deliverable structure.

## How the scope evolved

- The Terms of Reference (ToR) set a national coastal mandate.
- The literature review and inception process refined the focus using evidence.
- National mangrove extent mapping remained national in scope.
- Detailed socio-economic, ecosystem health, and carbon baselines focused on the most relevant mangrove landscapes.
- Muni-Pomadze was included in earlier phases but not all later technical phases because later evidence showed limited mangrove relevance.
- Keta became the pilot for project-specific MRV because it has the most complete layered baseline and monitoring package.
- The MRV system is national in framework, with project-specific hosting for places where detailed baselines exist.

## Deliverable Structure (confirmed 21 Mar 2026)

The assignment produces **four coordinated reports**:

| # | Report | Author | Status |
|---|---|---|---|
| 1 | **Blue Carbon Final Report** (this repo) | Team Leader | In progress |
| 2 | **MRV System Report** (standalone) | Team Leader | To be authored by Team Leader |
| 3 | **Drone Survey and EOSDA Continuous Monitoring Report** (standalone) | Team Leader | To be authored by Team Leader |
| 4 | **Carbon Inventory Report** (standalone) | Carbon Team | Pending Carbon Team delivery |

### Implications for Final Report chapters
- **Chapter 8** (Drone Survey and Continuous Monitoring): synthesis-level treatment; full technical detail is in the standalone Drone/EOSDA Report (Report 3). Chapter 8 does not replicate that report.
- **Chapter 9** (National MRV Framework and Keta Pilot): synthesis-level treatment; full technical and system detail is in the standalone MRV System Report (Report 2). Chapter 9 does not replicate that report.
- **Chapter 11** (Carbon Inventory Baseline): placeholder until the Carbon Team delivers Report 4.

## MRV System Repository

The Blue Carbon MRV system has its own GitHub repository: https://github.com/GAB-Climate-Smart/blue-carbon-mrv

### This repo is the primary source for the standalone MRV System Report (Report 2)
The Team Leader authors Report 2 separately from this repo.

### For the Final Report (Chapter 9), agents should draw on:
- Evidence packs already extracted: `evidence/mrv_system.md`, `evidence/mrv_repo_architecture.md`, `evidence/mrv_repo_dataflows.md`, `evidence/mrv_repo_pilot_logic.md`
- Visual exports when supplied by the Team Leader (not accessible via agent proxy)

### CRITICAL DISTINCTION
Treat the MRV repository as a **source of implementation detail ONLY**.
It is NOT the source of project scope authority.
Scope authority comes from the ToR, the inception report, and the synthesis of baseline evidence.

## Drone Survey and EOSDA

The standalone Drone Survey + EOSDA Continuous Monitoring Report (Report 3) is authored by the Team Leader. It covers:
- Drone orthomosaics and flight mission logs for survey plots
- EOSDA area-of-interest (AOI) setup and continuous hosting of drone AOIs
- Coverage maps and condition-mapping visual panels

Final Report Chapter 8 provides a synthesis-level summary and explicitly cross-references this standalone report for full technical detail.
