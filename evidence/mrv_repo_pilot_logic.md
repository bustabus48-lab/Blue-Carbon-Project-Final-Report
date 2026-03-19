# Evidence Pack: MRV Repo Pilot Logic (Keta within National Framework)

## 1) Does the repo support using Keta as a pilot?
- Yes, partially.
- Repo evidence includes Keta-specific onboarding traces (e.g., `seed_keta_mangrove.py`) and review notes that mention Keta/Songor hardcoded or semi-hardcoded baseline ingestion patterns.
- This supports a defensible interpretation that Keta-level implementation was used as an early operational entry point.

## 2) How a pilot can sit inside a national MRV framework
- The same repo contains national MRV framing documents (`docs/blueprint.txt`) and modular multi-domain schemas intended for broader use.
- A pilot-first model is therefore coherent: seed/project-area-specific onboarding in early phase, with migration toward generalized multi-project architecture (`projects` table wiring, project area typing, broader governance/compliance schemas).
- In reporting terms: pilot operations can validate workflows while the national architecture remains the governing frame.

## 3) Limitations that should be acknowledged in the report
- Repo review files explicitly signal MVP/prototype status and “needs hardening” in key audit-sensitive areas.
- Automated frequent satellite change-detection is described as incomplete/not fully automated.
- Baseline onboarding is not yet fully generalized in all review narratives; some scripts remain project-specific.
- Therefore, claims of fully mature nationwide continuous MRV operations should be avoided unless separately verified.

## 4) What the report can safely say
- “The MRV repository contains a national architecture design and working module scaffolding across geospatial, field, soil, carbon, safeguards, and compliance domains.”
- “Keta-linked onboarding artifacts support treatment of Keta as a practical pilot implementation context.”
- “The platform has demonstrable components (schema, roles, calculations, map-oriented modules), while full operational hardening is still indicated as ongoing in internal review documents.”
- “A pilot-first approach can coexist with a national framework where architecture is national and implementation depth matures site-by-site.”

## 5) What the report should not claim
- Do **not** claim the system is already fully audit-ready nationwide.
- Do **not** claim fully automated 7-day remote sensing classification is already operational unless external evidence confirms it.
- Do **not** claim all Ghana coastal districts can currently be onboarded through a complete no-code admin workflow.
- Do **not** claim pilot-specific scripts are evidence of uniform national implementation maturity.

## 6) Suggested caveat sentence for chapter drafting
- “Repository evidence indicates a functioning MRV prototype with strong national design intent and pilot-linked implementation traces; however, automation and audit hardening elements are still identified as in-progress in project review materials.”

## Primary repo artifacts reviewed
- `docs/PROJECT_REVIEW_GHANA_MRV.md`
- `docs/Final Mrv Review`
- `docs/blueprint.txt`
- `backend/scripts/seed_keta_mangrove.py`
- `supabase/migrations/*.sql`
- `supabase/functions/calculate-carbon/index.ts`
- `README.md`
