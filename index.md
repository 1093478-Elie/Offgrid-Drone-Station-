
---
Title: Off-Grid Solar Power System for Desert Environments
---

# Home

### Team Members:
* Abdullah Alhebshi ID: 1094916
* Mohammad Awab ID: 1094731
* Yunes Hussein ID: 1089060
* Elie Farah ID: 1093478

## Project Overview

Design and development of an off-grid solar power system for desert environments.

## Research Question

How can an off-grid solar power system be designed to maximize energy generation and ensure reliable battery storage and ensure reliable battery storage in desert environments.

## Project Status

| Work package | Status | Evidence |
|---|---|---|
| Background research and problem framing | Done | [Background Research](#background-research) |
| Measurable requirements and baseline | Done (draft) | [Updated Specifications](#updated-specifications) |
| Concept comparison and selection | Done (draft) | [Concept Selection](#concept-selection) |
| Preliminary calculations (4 analyses) | Done (draft, to be checked by team) | [Engineering Calculations](#engineering-calculations) |
| Risk register and safety plan | Done (draft) | [Safety and Risk Register](#safety-and-risk-register) |
| System architecture (power and control) | In progress | [System Design](#system-design) |
| Tracker CAD (3D concept model) | In progress | [Solar Tracker Design](#solar-tracker-design) |
| Bill of materials and budget | In progress | [Design and Manufacturing](#design-and-manufacturing) |
| Manufacture custom parts | Not started | |
| Electronics build and first feedback-loop demo | Not started | |
| Full integration and baseline test | Not started | |
| Validation (10 trials per condition) | Not started | |

**Overall: 5 of 12 work packages done, 3 in progress, 4 not started.** Design and planning are largely in place. The four remaining packages are the build, tuning and validation work.

Specification sign-off by the instructor is still pending.

## Background Research 

### YouTube Video 1

[Watch Video 1](https://www.youtube.com/watch?v=aHpVVMpBAfo)

### YouTube Video 2

[Watch Video 2](https://www.youtube.com/watch?v=MIAp5ZZ82mk&t=3s)

### Website Resource

[Dual Axis Solar Tracker System With Battery Charging](https://simplecircuitslol.blogspot.com/2025/11/dual-axis-solar-tracker-system-with.html)

## Technical Sources

- Sarver, Al-Qaraghuli and Kazmerski (2013), A comprehensive review of the impact of dust on the use of solar energy, Renewable and Sustainable Energy Reviews 22. Source for soiling losses and cleaning in desert sites.
- Duffie and Beckman, Solar Engineering of Thermal Processes (4th ed.). Source for the sun-angle and incidence-angle relations.
- PVGIS (European Commission JRC). Source for site irradiance data.

## Updated Specifications

Prototype requirements (scaled down from the capstone design)
| ID | Requirement | Target | How it is verified |
|---|---|---|---|
| R1 | Daily energy supplied to the loads (electronics plus one drone-battery top-up) | at least 15 Wh/day | Logged energy at the load |
| R2 | Energy gain of tracker vs the same panels locked at 35 degrees | at least +20% Wh/day (reported even if not met) | 10 trials per condition, mean and standard deviation |
| R3 | Pointing error of the tracker | at most 5 degrees (about 0.4% cosine loss) | Logged LDR error and reference sun angle |
| R4 | Tracker motion energy | at most 3% of energy generated | Logged servo current |
| R5 | Battery autonomy with no sun at 80% depth of discharge | at least 1 day | Discharge test at the design load |
| R6 | Battery temperature while charging | at most 45 degrees C, with a cutoff | Temperature log and cutoff check |
| R7 | Actuator torque with safety factor 2 | tilt axis at least 0.19 N·m, azimuth axis at least 0.37 N·m | Servo selection against Calculation 3 |
| R8 | Size | footprint within 240 x 200 mm base, height about 250 mm | CAD and measurement |
| R9 | Total budget | at most AED 800 | Final BOM |
| R10 | Electrical safety | 2S lithium-ion pack (7.4 V nominal, 8.4 V maximum) with protection circuit and fuse, emergency disconnect in under 1 s | Safety checklist |
Suggested targets and ensure that these are applicable

## Concept Selection

To be updated.

## System Design
<img width="1127" height="740" alt="12aa58ae-4c10-4d4c-8165-4be6244fbec2" src="https://github.com/user-attachments/assets/ab68b49b-a6e2-4f0c-9406-19529d804254" />

### Subsystems (From the CAD Model)


| Subsystem | Component | Notes |
|---|---|---|
| Generation | 2 solar panels, approximately 173 x 99 mm each, in a tilting tray | Total area 0.034 m^2 |
| Motion | Turntable (azimuth) and horizontal pivot shaft (tilt) with servo | Yoke holds the tray |
| Control | Arduino UNO class microcontroller, LCD status display | Display window in the enclosure front |
| Storage | Battery holder (75 x 38 x 23 mm) in the base | 2S lithium-ion pack, 2 x 18650 in series, 7.4 V nominal |
| Structure | Base enclosure 240 x 200 mm with removable lid | Houses electronics and battery |

## Solar Tracker Design

[Download Solar Tracker AutoCAD File (.DWG)](Solar%20Tracker%20PD.dwg)

## Engineering Calculations

To be updated.

## Design Optimization

To be updated.

## Design & Manufacturing

To be updated.

## Testing and Experimental Validation

To be updated.

## Presentation 1

Presentation slides link: To be updated.

Video Link: To be updated.

## Presentation 2

Presentation slides link: To be updated.

Video Link: To be updated.

## Bibliography

1. Sarver, T., Al-Qaraghuli, A., and Kazmerski, L. L. (2013). A comprehensive review of the impact of dust on the use of solar energy: history, investigations, results, literature, and mitigation approaches. *Renewable and Sustainable Energy Reviews*, 22, 698-733.
2. Duffie, J. A., and Beckman, W. A. (2013). *Solar Engineering of Thermal Processes* (4th ed.). Wiley.
3. European Commission Joint Research Centre. PVGIS (Photovoltaic Geographical Information System), for site irradiance data.
4. Video 1, Video 2 and the dual-axis tracker blog post listed under Background Research.
