# Evidence Pack: MRV Repository Dataflows (for Report Authors)

## 1) What data appears to enter the system
Visible repo artifacts indicate incoming data categories:
- Spatial baseline and monitoring layers (GeoJSON polygons for plots/project areas/buffers/leakage zones).
- Field biomass measurements tied to sample plots.
- Soil sample records with lab analysis fields and derived soil-carbon density.
- Emission factors by mangrove stratum.
- Alerts/classification-run metadata and map-layer references.
- Leakage/permanence records (market surveys, reversal events, risk scoring entries).
- Safeguards/compliance records (FPIC-style docs, grievance/compliance-cycle evidence fields).

## 2) How data is stored, displayed, updated, or monitored (observable in repo)
### Storage model (observable)
- Supabase/PostgreSQL + PostGIS is the stated backend pattern.
- Migrations show dedicated tables by domain (plots, soil, carbon accounting, safeguards, compliance, project areas, operational governance).
- Row-level security policies are present across many tables (role-scoped data access).

### Processing/update model (observable)
- Carbon engine function (`calculate-carbon`) reads latest plot + measurement + soil + emission factor entries and writes a calculation record with deductions.
- Seed script evidence shows manual/project-specific baseline ingestion path (hardcoded local file path in current script snapshot).
- CI/deploy flow is documented, but does not by itself prove live production data automation.

### Display/monitoring model (observable via repo docs)
- Repo review docs describe map/dashboard modules that visualize polygons/alerts/compliance sections.
- Review docs also state some sections still rely on placeholders or require hardening for audit-grade use.

## 3) Visible assumptions, dependencies, and limitations
### Assumptions/dependencies
- Supabase credentials and environment variables are required.
- GeoJSON and table schemas must be loaded/migrated before higher-level functions operate.
- Emission factors are required for carbon calculations (with “Default” fallback logic in function code).

### Limitations/uncertainties flagged by repo itself
- Automated recurring satellite-classification pipeline is described as not fully implemented in review notes.
- Baseline ingestion appears partly script-dependent and not yet fully generalized via admin UI workflows.
- “National performance” targets in blueprint text are requirements/targets, not confirmed runtime evidence in this review pass.

## 4) Where drone, monitoring, and baseline layers appear to fit
- Drone/boundary-derived polygons appear to fit in project area and map-layer ingestion pathways (GeoJSON upload + project area typing).
- Monitoring observations appear to fit in sample plots, measurements, soil samples, and alert/compliance cycle records.
- Baseline layers appear to fit as initial project-area/strata/classification tables used for ongoing updates and derived calculations.
- Important caution: repo evidence supports the **data structure for this flow**; it does not fully prove automated, nationwide recurring ingestion is already operational.

## 5) Reporting-safe phrasing cues
- “The repository implements multi-domain storage structures and workflow scaffolding for MRV data integration.”
- “Some modules are operational at prototype/MVP level, while automation and audit hardening remain in-progress per internal review notes.”

## Primary repo artifacts reviewed
- `README.md`
- `docs/PROJECT_REVIEW_GHANA_MRV.md`
- `docs/Final Mrv Review`
- `docs/Data Requirements`
- `supabase/migrations/*.sql`
- `supabase/functions/calculate-carbon/index.ts`
- `backend/scripts/seed_keta_mangrove.py`
