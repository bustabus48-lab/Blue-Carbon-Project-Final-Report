# Technical Report: Drone Survey & EOSDA Continuous Monitoring Baseline (2026)

## Technical Report: Drone Survey & EOSDA Continuous Monitoring Baseline (2026)

## 1. Executive Summary
This technical report documents the establishment of a high-resolution drone-derived baseline and the integration of continuous satellite monitoring for the Keta Lagoon Complex. The operational framework identifies 1,467.0 hectares of priority mangrove systems across four distinct Areas of Interest (AoIs). These areas serve as the initial "Gold Standard" monitoring units for the National Blue Carbon MRV Platform.

**Selected Drone Survey AoIs (2026 Baseline)**
| Area of Interest | Strategic Cluster | Area (Ha) | Core Classification |
|---|---|---|---|
| Aborlove Nolopi | Eastern Cluster | 52.0 | Mixed (Degraded & Intact) |
| Agatsivi-Agortoe | Central Cluster | 762.0 | Contiguous / Fragmented |
| Salo-Agortoe Stretch | Central Cluster | 525.0 | Creek System / Near-Community |
| Anyanui Combine | Western Cluster | 128.0 | Restoration Potential |
| **TOTAL** | | **1,467.0** | |

## 2. Drone Survey Methodology
The drone survey campaign utilized high-resolution multispectral sensors (MicaSense/Phantom 4 Multispectral) to establish a 2026 "Zero Point" baseline.

### 2.1 Survey Objectives
* **Orthomosaic Calibration:** Establishing `keta_lagoon.tif` as the master spatial reference.
* **Micro-Topography:** Mapping drainage density within the Salo-Agortoe creek systems.
* **Species Identification:** Resolving _Avicennia germinans_ vs. _Rhizophora mangle_ spectral signatures at 5cm-10cm GSD.

### 2.2 Flight Parameters
* **Altitude:** 100m - 120m AGL.
* **Overlap:** 80% Front / 75% Side.
* **Ground Control Points (GCPs):** Minimum 5 per AoI for centimeter-level accuracy (RTK-corrected).

## 3. EOSDA Monitoring Architecture
The drone-derived polygons are ingested into the EOS Data Analytics (EOSDA) platform to enable automated, continuous monitoring via Sentinel-2 (10m resolution).

### 3.1 Satellite Workflow
* **Frequency:** Automated scan every 3-5 days.
* **Indices:** Normalized Difference Moisture Index (NDMI) for stress detection and NDVI for biomass trends.
* **Alert Logic:** Automatic notifications triggered when NDMI deviance exceeds 15% from the moving average (indicating potential clearing or dieback).

### 3.2 Ingested Boundary Features
The platform tracks the following NDMI-linked units:
- **Dzita North/South/West:** Restoration zones.
- **Salo PSP 1:** Permanent Sample Plot monitoring.
- **Aborlove/Anyanui:** Jurisdictional monitoring stretches.

## 4. Institutional Transition & Handover
This monitoring system is designed for handover to the **Ministry of Environment, Science, Technology and Innovation (MESTI)** and the **Environmental Protection Agency (EPA)**.

### 4.1 Technical Operations
1. **Platform Access:** GAB Corporate EOSDA portal integration.
2. **Dashboard Management:** Real-time visualization of `gab-ramsar-map` data layers.
3. **Field Verification:** CCAs (Community Change Agents) utilize the MRV Mobile App to verify sat-alerts on the ground.

### 4.2 Data Governance
All spatial assets, including the `aborlove-nowlopi-mangrove.kml` and `agatsivi-agortoe-stretch.kml` source files, are archived in the National Blue Carbon Registry.

---
*Report Status: Draft V1.0*
*Source Repositories: [blue-carbon-mrv](https://github.com/GAB-Climate-Smart/blue-carbon-mrv), [gab-ramsar-map](https://github.com/GAB-Climate-Smart/gab-ramsar-map)*
