# Drone Survey and EOSDA Continuous Monitoring Report — Standalone Report Outline

**Author:** Team Leader (to be authored independently)
**Status:** Stub / outline — content to be produced by Team Leader
**Cross-reference:** Final Report Chapter 8 synthesises from this report

---

## Purpose of This Document
This outline defines the structure and content requirements for the standalone Drone Survey and EOSDA Continuous Monitoring Report. This is a separate deliverable from the Blue Carbon Final Report. The Team Leader authors it independently, drawing on drone survey outputs, EOSDA platform configuration, and monitoring data generated during the assessment.

---

## Suggested Structure

### 1. Introduction
- Purpose of the drone survey programme within the blue carbon assessment
- Purpose of EOSDA continuous monitoring and how it extends the assessment beyond the field campaign
- Relationship to the Blue Carbon Final Report and MRV System

### 2. Drone Survey Programme

#### 2.1 Survey Design
- Survey areas and rationale for site selection
- Drone equipment and flight specifications
- GSD (ground sampling distance), overlap, altitude parameters
- Flight authorisation and safety considerations

#### 2.2 Survey Coverage
- Map of all surveyed areas with acquisition dates
- Total area surveyed per site
- Coverage relative to assessment sampling extent

#### 2.3 Products Generated
- Orthomosaic products (overview panel with acquisition date labels)
- Digital surface models (if generated)
- Condition classification or canopy-mapping outputs derived from imagery
- Sample plot boundary overlays

#### 2.4 Quality and Accuracy Assessment
- Ground control points used (if any)
- Positional accuracy achieved
- Known coverage gaps and reasons

### 3. EOSDA Continuous Monitoring Setup

#### 3.1 Platform Overview
- EOSDA platform description and capability used
- Subscription / account configuration for this programme

#### 3.2 Areas of Interest (AOIs) Configured
- List and map of all AOIs set up
- AOI polygon sources (drone-derived, field-mapped, or desk-delineated)
- Date AOIs were activated

#### 3.3 Monitoring Parameters and Indices
- Vegetation indices monitored (NDVI, EVI, etc.)
- Flood / inundation monitoring configuration
- Alert thresholds or change-detection settings

#### 3.4 Monitoring Outputs to Date
- Time-series charts or outputs for key AOIs since activation
- Any alerts or anomalies detected
- Screenshots of EOSDA monitoring dashboard for key AOIs

#### 3.5 Linkage to MRV System
- How EOSDA outputs are exported and ingested into the MRV system
- Current automation level and manual steps

### 4. Interpretation: What the Data Show
- Summary of condition signals visible in drone imagery
- Summary of any change signals detected via EOSDA since monitoring began
- Key observations relevant to restoration and protection planning

### 5. Limitations and Recommendations
- Survey coverage gaps and implications for monitoring completeness
- Seasonality considerations for EOSDA monitoring interpretation
- Recommended revisit frequency for drone surveys
- Recommended AOI refinements or additions for next monitoring cycle

### 6. Annexes
- A. Flight log table (date, site, area, GSD, operator)
- B. AOI configuration table (name, area, activation date, indices monitored)
- C. Orthomosaic index (file names, dates, GSD, site)
- D. Full-resolution orthomosaic panels (or link to data storage)

---

## Visual Assets Required
The following visuals must be prepared and inserted before finalisation:

| Asset | Description | Section |
|---|---|---|
| Survey coverage map | All surveyed areas with acquisition dates | §2.2 |
| Orthomosaic collage panel | Representative imagery from each site | §2.3 |
| Condition classification panel | Canopy/condition mapping output | §2.3 |
| EOSDA AOI map | All configured AOIs on coastal basemap | §3.2 |
| EOSDA dashboard screenshot | Active monitoring view for a key AOI | §3.4 |
| NDVI or index time-series | Chart showing monitoring signal since activation | §3.4 |

---

## Notes for the Team Leader
- Export orthomosaics from the drone processing software (DJI Terra, Pix4D, OpenDroneMap, or equivalent).
- Export EOSDA monitoring screenshots and time-series charts from the EOSDA platform dashboard.
- Confirm AOI polygon sources — if any polygons were derived from the `blue-carbon-mrv` repository spatial data, note this linkage.
- Once this report is drafted, notify the writing agent so Chapter 8 of the Final Report can be updated with confirmed claims and actual visual inserts.
