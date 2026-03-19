# Evidence Pack: Drone Survey Outputs and Spatial Monitoring Readiness

## Chapter Purpose (for later drafting)
This pack captures evidence on drone-linked spatial products, named monitoring polygons/plots, and operational monitoring design signals.  
It should support chapter drafting on readiness and data assets, without claiming results that are not explicitly documented.

## Core Findings (traceable)
- ToR requires baseline maps to be annexed with drone/aerial shots of current area conditions, stored in a database. (Source: `terms_of_reference_revised_mlnr.md` — “Phase 3: Development of baseline Land Cover /land use change Maps”).
- Blue carbon final report blueprint defines a dedicated chapter on drone outputs, emphasizing orthomosaics, plot imagery, boundary refinement, and condition mapping as transition-to-monitoring outputs. (Source: `blue_carbon_final_report_blueprint.md` — “Chapter 6. Drone Survey Outputs and Spatial Monitoring Readiness”).
- Monitoring plan for Keta and Ada defines supervised-map-based sampling design and quarterly field monitoring cycle, indicating readiness for recurring geospatially anchored monitoring. (Source: `monitoring_plan_for_keta_and_ada.md`).
- Repository contains dated site polygons indicative of drone/NDMI output products and monitoring units, including restoration and protection areas and a permanent sample plot boundary. (Source: boundary files in `source_reports/`).

## Approved Numbers, Named Sites, Dates, Definitions
### Approved numbers currently extractable
- Sampling sites in monitoring plan: 57 (Keta) and 23 (Ada), with quarterly schedule. (Source: `monitoring_plan_for_keta_and_ada.md`).
- Geojson polygon files detected: 7 boundary datasets with one feature each. (Source: repository file inventory and boundary file properties).

### Named drone/monitoring polygons from source filenames/properties
- `Dzita_Restoration_Areas_NDMI_03Mar2026`
- `Salo_Restoration_Area_NDMI_26Feb2026`
- `Salo_Permanent_Sampla_Plot_1_NDMI_03Mar2026`
- `Avu_Protection_Area_NDMI_21Feb2026`
- `Aborlove_Protection_Area_NDMI_26Feb2026`
- Keta lagoon boundary datasets (Ramsar and lagoon boundary variants)
(Sources: corresponding `.geojson` and `.kml` boundary files in `source_reports/`).

### Dates
- Dated polygon names indicate monitoring product windows in Feb-Mar 2026.
- Monitoring plan references assessment context in December 2025.

### Definitions/terms to preserve
- “Permanent Sample Plot” (PSP) appears in spatial product naming and MRV design docs.
- “NDMI” appears in polygon labels and should be retained as dataset identifier unless expanded in source method notes.

## National vs Site-Specific Distinction (must preserve)
- National requirement: drone/aerial evidence integration within baseline and monitoring architecture.
- Site-specific implementation evidence currently strongest for Keta-linked and nearby named polygons; do not extrapolate equal drone detail to all national coastal areas.

## Most Relevant Source Files Used
- `source_reports/terms_of_reference_revised_mlnr.md`
- `source_reports/blue_carbon_final_report_blueprint.md`
- `source_reports/monitoring_plan_for_keta_and_ada.md`
- `source_reports/dzita_restoration_areas_ndmi_03mar2026_boundary.geojson`
- `source_reports/salo_restoration_area_ndmi_26feb2026_boundary.geojson`
- `source_reports/salo_permanent_sampla_plot_1_ndmi_03mar2026_boundary.geojson`
- `source_reports/avu_protection_area_ndmi_21feb2026_boundary.geojson`
- `source_reports/aborlove_protection_area_ndmi_26feb2026_boundary.geojson`
- `source_reports/keta_lagoon_boundary.geojson`
- `source_reports/keta_lagoon_ramsar_boundary.geojson`

## Figures and Tables to Use
- Map panel of all available named NDMI polygons and Keta boundary layers.
- Table: polygon name, type (restoration/protection/PSP/boundary), date encoded in name, source file.
- Process figure: baseline mapping -> drone/NDMI products -> quarterly field sampling loop.

## Known Gaps / Open Questions
- No extracted drone mission logs, flight specs, orthomosaic metadata, or sensor parameters found in currently parsed text sources.
- Need explicit linkage table between each polygon and field implementation status (planned/active/completed).
- Need confirmation of how Ada monitoring units align with Songor Ramsar nomenclature in chapter text.

## Writing Constraints (do not overclaim)
- Do not claim drone-derived area statistics or accuracy metrics unless explicitly documented.
- Do not claim full national drone coverage; current explicit polygon evidence is site-specific.
- Do not treat filename date stamps as completion dates without confirmation.
- Do not infer ecological outcomes from polygon existence alone.
