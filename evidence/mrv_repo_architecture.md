# Evidence Pack: MRV Repository Architecture (for Report Authors)

## Scope of this evidence pack
This pack summarizes what is visible in the `GAB-Climate-Smart/blue-carbon-mrv` repository and its embedded review documents.  
It is written for report drafting support (not engineering implementation guidance).

## 1) System purpose (plain language)
- The repository describes an integrated Blue Carbon MRV platform intended to track monitoring, reporting, verification, safeguards, and compliance evidence in one system.
- The stated policy intent (in repo documents) is national-level MRV support, while implementation artifacts include specific project-area onboarding and pilot-style baseline data flows.

## 2) Major modules / features visible in repo evidence
Based on `README.md`, `docs/blueprint.txt`, and migration/module files, visible module areas include:
- User management and governance (roles, access control, audit intent).
- Plot and field data management (sample plots, measurements).
- Soil/laboratory records (soil sample chain-of-custody style fields).
- GIS/spatial data layers (mangrove plots, leakage zones, project areas, geojson views).
- Alerts/change-monitoring records (SAR/NDVI-related alert tables and classification run scaffolding).
- Carbon accounting (emission factors, calculations, deductions, results storage).
- Leakage/permanence records (market surveys, reversal events, risk scoring).
- Safeguards/social integrity (FPIC-type documents, grievance records).
- Compliance/traceability cycle scaffolding (monitoring cycles, checklist status).
- Registry interface intent (export-oriented in docs; minimal integration positioning).

## 3) What appears operational vs conceptual/planned
### Appears implemented (or partially implemented in schema/UI terms)
- Core stack and deployment scaffolding are present (frontend, backend, supabase, CI/deploy references in README).
- Multiple domain tables/migrations exist across geospatial, soil, carbon, safeguards, leakage, compliance, and project-area modules.
- A working carbon calculation edge-function exists that reads plot/measurement/soil/emission-factor tables and writes calculation outputs.
- Repo review docs state dashboard/map modules exist and some upload/document persistence is in place.

### Appears conceptual, incomplete, or “needs hardening”
- Repo’s own review files classify the platform as MVP/prototype, not yet production-ready for national MRV audits.
- Automated 7-day classification workflow is repeatedly flagged as not yet end-to-end operational.
- Baseline ingestion for arbitrary Ghana coastal areas is flagged as partially met and environment-dependent.
- Cross-module audit traceability and immutable evidence linkage are described as incomplete in review notes.

## 4) What supports national baseline framing
Evidence in repo that supports national framing:
- RFP/ToR-style blueprint in `docs/blueprint.txt` is explicitly framed as a National Blue Carbon MRV digital platform.
- README and docs repeatedly describe national MRV alignment and government/internal institutional roles.
- Schema evolution includes generalized `projects` wiring and governance/monitoring cycles that can support multi-project architecture.

## 5) What supports project-specific hosted baselines
Evidence in repo that supports project-specific hosted baselines:
- Seed and review materials reference specific landscape onboarding (e.g., Keta/Songor context and project-area uploads).
- `project_areas` schema explicitly supports typed polygons (`restoration`, `conservation`, `protection`, `buffer`, `reference`) for hosted project layers.
- Data-input docs list concrete project boundary and sample plot inputs for specific landscapes.

## 6) Evidence strength notes (for cautious drafting)
- Strongest evidence: module presence, schema structures, and self-assessment status from repo review docs.
- Weaker evidence: real operational uptime/performance against national SLA targets; this is stated as target/requirement in blueprint text and not independently verified here.
- Report wording should therefore distinguish between “designed/intended capability” and “currently operational capability.”

## Primary repo artifacts reviewed
- Root `README.md`
- `docs/PROJECT_REVIEW_GHANA_MRV.md`
- `docs/Final Mrv Review`
- `docs/Data Requirements`
- `docs/blueprint.txt`
- `supabase/migrations/*.sql` (module-specific migrations)
- `supabase/functions/calculate-carbon/index.ts`
- `backend/scripts/seed_keta_mangrove.py`
- `.env.example`, `docker-compose.yml`
