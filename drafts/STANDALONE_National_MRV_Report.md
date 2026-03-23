# Standalone National MRV Report

**Draft status:** working draft for authoring and evidence extraction  
**Primary evidence files used:** `source_reports/blue_carbon_mrv_report.md`; `evidence/mrv_system.md`; `evidence/mrv_repo_architecture.md`; `evidence/mrv_repo_dataflows.md`; `evidence/mrv_repo_pilot_logic.md`; `qa/scope_logic_note.md`  
**Major known gaps:** Final dashboard screenshots, hotspot/alert exports, role-view exports, finalized data dictionary, and independent confirmation of full operational deployment are not yet available in the repository.

## 1. Executive Summary
This report presents the current draft of Ghana’s National Blue Carbon Monitoring, Reporting, and Verification (MRV) framework as a standalone source report for the wider Blue Carbon Final Report package. Available evidence supports a national MRV design that integrates ecological and carbon monitoring, environmental pressure surveillance, and governance and safeguard assurance within one framework.

The source evidence indicates that the MRV design is structured around four institutional tiers: community level, district level, national technical level, and independent review where required. It also indicates three functional layers: ecological and carbon integrity, environmental pressure surveillance, and governance and safeguard assurance. Together, these layers are intended to support recurring observation, transparent reporting, and long-term management of blue carbon landscapes.

The current evidence base is strong on framework design, indicator logic, and intended digital architecture. It is weaker on proof of fully operational national deployment. Repository evidence also supports treatment of Keta as an early pilot implementation context within the broader national framework, but not as a substitute for national scope.

Accordingly, this report distinguishes clearly between completed design evidence, pilot-linked implementation traces, and pending operational proof.

## 2. Purpose and Scope of This Standalone Report
The purpose of this standalone report is to:
- set out the documented design of the national MRV framework;
- summarize the institutional architecture, indicators, governance logic, and data flows already evidenced in source materials;
- explain how a pilot implementation context can sit within a national system design; and
- provide a clean markdown source report that can be used for evidence extraction and integration into the Final Report.

This report is not presented as proof that the MRV system is already fully operational nationwide. It is a draft evidence-based account of the framework design and the implementation maturity that can currently be supported by the repository.

## 3. Strategic Context and Design Intent
The MRV source report positions Ghana’s coastal wetlands and mangrove ecosystems as nationally significant assets for climate regulation, biodiversity protection, shoreline stabilization, fisheries support, and livelihood security. Within that frame, the MRV framework is intended to provide an institutional and technical basis for:
- monitoring mangrove and coastal wetland extent and condition;
- quantifying and tracking carbon stocks and emission reductions;
- detecting degradation pressures and triggering response;
- supporting safeguards, transparency, and inclusive governance; and
- improving the credibility of blue carbon investment and reporting.

The framework is informed by a broader baseline package that includes geospatial extent mapping, ecosystem health analysis, socio-economic profiling, environmental pressure assessment, governance-readiness work, and carbon inventory design. This means the MRV framework should be read as one component of an integrated national monitoring architecture rather than as an isolated technical system.

## 4. Institutional Architecture
Available evidence supports a four-tier institutional structure.

### 4.1 Community level
Community Resource Management Areas (CREMAs) and community change agents are intended to support field-based observation of restoration activity, degradation signals, and some governance-related indicators.

### 4.2 District level
Metropolitan, Municipal, and District Assemblies (MMDAs), together with the Wildlife Division and related local structures, are expected to consolidate field data, support validation, and contribute to conflict handling and reporting.

### 4.3 National technical level
The Ministry of Lands and Natural Resources (MLNR), Ministry of Environment, Science, and Technology (MEST), Forestry Commission (FC), and other national technical actors are intended to provide GIS analysis, carbon stock oversight, QA/QC, national data archiving, and reporting.

### 4.4 Independent review
Independent verification is included where required, particularly in contexts where carbon market participation or third-party assurance would apply.

## 5. Functional Layers and Indicator Logic
The MRV framework is documented as operating through three linked functional layers.

| Functional layer | What it covers | Evidence-backed signals |
|---|---|---|
| Ecological and carbon integrity | Mangrove extent, restoration performance, carbon stocks, and long-term asset integrity | National baseline reference, annual extent monitoring, PSP logic, carbon pool tracking |
| Environmental pressure surveillance | Drivers of degradation and early warning signals | Land conversion, mangrove cutting signals, fuel-source shift, charcoal hotspots, conflict/access pressure |
| Governance and safeguard assurance | Participation, benefit transparency, conflict monitoring, grievance handling, and safeguards | Representation targets, grievance tracking, benefit-sharing documentation |

The indicator logic already evidenced in the repository includes:
- annual satellite-based mangrove and wetland extent monitoring;
- biomass remeasurement every 3-5 years;
- soil carbon reference depth of 0-100 cm;
- quarterly and annual pressure-monitoring cycles for selected field and governance indicators;
- weekly satellite-feed updates in the intended digital platform design; and
- a minimum 40% female representation target in executive leadership under the governance-monitoring logic.

The source evidence also indicates annual household-sampling guidance of 20-30 households per CREMA for fuel-shift monitoring in the environmental pressure layer.

## 6. National Baseline Reference and Monitoring Cycles
The MRV evidence identifies the 2025 baseline package as the Year 0 reference for future measurement and benchmarking. This baseline reference is important because it anchors future claims about:
- mangrove spatial coverage;
- ecosystem classification and stratification;
- fragmentation and restoration opportunity mapping; and
- carbon stock remeasurement.

The report should therefore preserve the distinction between:
1. the baseline reference package already used to design the framework; and
2. future recurring monitoring outputs that would demonstrate operational performance over time.

## 7. Digital Platform and Data Flow
Available evidence describes an intended digital platform that combines spatial monitoring, field observations, carbon data, safeguards, and reporting logic.

At a reporting-safe level, the repository evidence supports the following statements:
- the platform architecture is intended to host spatial layers, plots, project areas, soil records, carbon calculations, safeguards evidence, and compliance records;
- role-based access control and audit-oriented workflow structures are present in the repository design evidence;
- carbon-calculation functions and multiple domain tables are visible in repository review materials;
- drone- and boundary-derived polygons are intended to enter the platform through project-area and map-layer ingestion pathways; and
- the data structure supports an integrated flow from field and spatial inputs to reporting outputs.

The intended reporting pathway can be summarized as:

**Community / field observation -> district consolidation and validation -> national technical QA/QC and storage -> platform visualization / analysis -> reporting and management response**

This data-flow logic is well supported at design level. It is less well supported as proof of full national runtime automation.

## 8. What Appears Implemented and What Remains In Progress
The current evidence supports a cautious two-level reading of MRV maturity.

### 8.1 Components that appear implemented or demonstrable
- multi-domain schema structures across geospatial, field, soil, carbon, safeguards, leakage, and compliance functions;
- core stack and deployment scaffolding;
- a working carbon-calculation function in repository evidence;
- documented map and dashboard module intent; and
- project-area onboarding traces that support pilot-linked implementation narrative.

### 8.2 Components still described as incomplete, prototype-level, or requiring hardening
- fully automated recurring remote-sensing classification workflows;
- generalized baseline onboarding for arbitrary coastal areas through fully mature workflows;
- complete audit-grade traceability and immutable evidence linkage across modules; and
- independently verified proof of full national operational deployment.

For this reason, the safest report wording is that the current evidence indicates a **functioning MRV prototype with strong national design intent and pilot-linked implementation traces**, while automation and audit hardening remain in progress.

## 9. Keta as Pilot Implementation Context
The evidence supports a pilot-first interpretation in which Keta is treated as an early implementation context nested inside the broader national MRV framework. This interpretation is based on:
- stronger layered baseline evidence associated with Keta;
- repository onboarding traces linked to Keta;
- the monitoring and plot logic that is most visible for Keta-linked contexts; and
- the broader scope notes that explicitly preserve national architecture while allowing site-specific implementation depth to mature unevenly.

This pilot framing should be used carefully. It is appropriate to say that Keta provides an early operational test bed or implementation context. It is not appropriate to imply that Keta-level readiness automatically proves equal readiness across all blue carbon landscapes in Ghana.

## 10. Governance, Safeguards, and Reporting Assurance
An important strength of the MRV framework design is that it does not treat carbon accounting as separate from governance and safeguards. The documented framework includes:
- representation and inclusion monitoring;
- grievance redress tracking;
- benefit-transparency logic;
- conflict monitoring; and
- QA/QC and reporting structures intended to support accountability.

This should remain central to how the MRV report is framed. The national MRV framework is not only a technical measurement system; it is also a governance and assurance architecture for blue carbon management.

## 11. Evidence Boundaries and Drafting Constraints
This draft should preserve the following constraints:
- do not claim the MRV system is already fully operational nationally unless deployment evidence is provided;
- do not claim third-party verification or carbon-market issuance outcomes unless the relevant source documents are available;
- do not treat pilot-specific scripts or onboarding traces as proof of uniform nationwide implementation maturity;
- do not allow repository implementation details to redefine the formal scope authority of the consultancy; and
- do not convert design intent into confirmed implementation outcome without direct supporting evidence.

## 12. Placeholder Requirements Before Final Publication
**[PLACEHOLDER NOTE – REQUIRED BEFORE FINAL PUBLICATION]**

Insert the following if and when they are available:
- MRV dashboard screenshot(s) showing national overview;
- hotspot or alert export(s);
- representative workflow or role-view export(s);
- final data dictionary and indicator metadata tables; and
- any approved statement on formal adoption or deployment status.

Until these are available, visual and operational language should remain cautious and evidence-limited.

## 13. Decisions, Pending Inputs, and Next Actions
### Completed evidence
- National MRV design report exists in markdown.
- Institutional architecture and functional-layer logic are clearly documented.
- Core monitoring frequencies, carbon-pool references, and governance signals are extractable.
- Repository evidence supports a coherent national architecture with pilot-linked implementation traces.

### Pending inputs
- final screenshots and system exports for visual proof;
- final deployment-status confirmation;
- final data dictionary and annex-ready indicator tables; and
- any confirmation of legal or institutional adoption status beyond the current draft-design stage.

### Next actions
1. Use this draft as the standalone markdown source report for extraction and final-report synthesis.
2. Add annex-ready diagrams and tables when screenshots and metadata are available.
3. Keep Keta references framed as pilot implementation context within national architecture.
4. Update the operational-status section only when direct proof is added to the repository.
