# Chapter 9. National MRV Framework and Keta Pilot

**Draft status:** synthesis summary — awaiting standalone companion report for visual exports
**Primary evidence files used:** `evidence/mrv_system.md`; `evidence/mrv_repo_architecture.md`; `evidence/mrv_repo_dataflows.md`; `evidence/mrv_repo_pilot_logic.md`; `qa/scope_logic_note.md`; `qa/chapter_traceability_map.md`
**Companion report:** _MRV System Report_ (standalone, authored by Team Leader). Full system architecture, data model, workflow logic, and visual exports are in that report. This chapter provides a synthesis-level treatment and explicit cross-reference.
**MRV repository:** `GAB-Climate-Smart/blue-carbon-mrv`

---

## 9.1 Chapter Purpose and Scope
This chapter describes the national blue carbon MRV framework designed for Ghana and the Keta pilot implementation that demonstrates the framework in operation. It presents the governance logic, architecture overview, and the sequencing rationale that positions Keta as the initial operational context within a national system.

Full system documentation — including architecture diagrams, data models, workflow logic, role-access design, dashboard exports, and operational configuration detail — is contained in the standalone **MRV System Report**, authored by the Team Leader and drawing on the `GAB-Climate-Smart/blue-carbon-mrv` repository. Readers requiring technical system detail should refer to that companion report.

## 9.2 National MRV Framework: Design and Rationale
The national MRV framework provides a structured, standards-aligned mechanism for tracking changes in blue carbon ecosystems across Ghana's coastal zone. The framework integrates:

- **Multi-layer monitoring:** Combining satellite remote sensing (including EOSDA-hosted AOIs), drone survey outputs, field-collected ecological and soil parameters, and socio-economic indicators into a coherent monitoring stream.
- **Institutional tiering:** Governance structured across national (MESTI), site-level, and community stakeholder tiers, with defined roles for data submission, validation, and reporting at each level.
- **Indicator-based reporting cycles:** Recurring reporting cycles anchored to verified ecological and carbon stock indicators, designed to be consistent with international standards for blue carbon accounting.
- **Safeguards and transparency:** Explicit safeguards architecture and transparent data provenance, aligned with REDD+ and international climate reporting requirements.

## 9.3 Keta as Pilot Implementation Context
Keta was selected as the pilot implementation context on the basis of evidence-led sequencing: it holds the most complete layered baseline among the assessed landscapes, combining mangrove extent data, ecosystem health parameters, carbon inventory work, drone survey coverage, and the deepest socio-economic characterisation.

The pilot treatment means:
- Keta-specific data flows are the first to be configured and tested within the MRV system architecture.
- Operational outputs — including monitoring dashboards, alert logic, and reporting modules — have been tested against Keta data before wider roll-out.
- Lessons from the Keta pilot are expected to inform onboarding of additional landscapes as their baselines mature.

This is implementation sequencing, not scope substitution. The national framework applies across all assessed coastal landscapes; Keta is the leading operational instance.

## 9.4 System Architecture: Summary
The MRV system (`GAB-Climate-Smart/blue-carbon-mrv`) is a web application providing national-level monitoring oversight with site-level drill-down. At architecture level it integrates:

- **Data ingestion and processing modules:** Automated and semi-automated pipelines for spatial data, field observations, and remote sensing inputs.
- **Indicator computation and storage:** A structured data model supporting carbon stock estimates, ecosystem condition indicators, and pressure tracking.
- **Dashboard and reporting interface:** User-facing views for national overview, site-level detail, and alert/hotspot monitoring.
- **Role-based access:** Differentiated access for national administrators, site-level data managers, and read-only stakeholder views.

Architectural detail, schema diagrams, and data flow logic are documented fully in the standalone MRV System Report and in the repository.

## 9.5 Operational Status: Honest Framing
Available evidence supports the presence of core system components, schema structures, and processing modules. Some elements remain at prototype or active-hardening stage as of this report. Accordingly:

- Claims of **implemented and demonstrable** capability apply where evidence is direct (architecture, data model, pilot data integration).
- Claims of **design intent or in-progress capability** apply where full operational proof is not yet available.

This framing will be updated when the Team Leader completes the standalone MRV System Report and confirms operational status for each component.

## 9.6 Cross-Reference to Standalone Companion Report
Full documentation of the following is in the standalone _MRV System Report_:

- system architecture diagrams and data model;
- workflow logic and role-access design;
- MRV dashboard screenshots (national overview, site-level, hotspot/alert views);
- data dictionary and field definitions;
- operational configuration and hosting details.

**[INSERT BEFORE FINAL LAYOUT]** Representative dashboard screenshot (national overview), site-level monitoring panel, and hotspot/alert export should be drawn from the standalone MRV System Report and inserted here. Provide these assets to the writing agent when the standalone report is finalised.

## 9.7 Forward Path
The national MRV framework and Keta pilot together provide a credible foundation for phased operational expansion. As additional landscape baselines mature — including Songor, Ada, and other coastal sites — the MRV system architecture is designed to accommodate progressive onboarding. The standalone MRV System Report details the technical roadmap for this expansion.
