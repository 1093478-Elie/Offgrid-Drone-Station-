
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

Design and development of an off-grid solar power station for a drone docking in a desert environment (UAE conditions). A dual-axis solar tracker provides power to the lithium-ion battery (the backup battery in the capstone), which can power the drone's dock and hub. The project is a scaled prototype of our full design in the capstone.

**Scope:** The prototype is tested under controlled and outdoor environments. It uses low voltage DC only.

## Research Question

How can an off-grid solar power system be designed to maximize energy generation and ensure reliable battery storage and ensure reliable battery storage in desert environments.

**Hypothesis:** A dual-axis tracker that points the panel at the sun will generate at least 20% more energy per day than the panels that are constant.

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

To be Updated

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

### Control Architecture

To be updated.

### Power Architecture

To be updated.

## Solar Tracker Design

[Download Solar Tracker AutoCAD File (.DWG)](Solar%20Tracker%20PD.dwg)

| Part | Dimensions |
|---|---|
| Base enclosure | 240 x 200 x 52 high, 3 mm floor, 3 mm walls |
| Removable lid | 240 x 200 x 4 |
| Turntable | diameter 140, height 12 |
| Yoke crosspiece | 226 x 70 x 8 |
| Yoke arms | 8 x 50 x 122 high, two arms |
| Pivot shaft (hardware) | diameter 8, length 226, at 183 mm height |
| Panel tray | 185 x 218 outer, tilted 35 degrees in the model |
| Solar panels | 2 x (173 x 99 x 2) |
| Electronics placeholders | UNO 69 x 54 x 16, LCD window 80 x 36, battery holder 75 x 38 x 23 |

## Engineering Calculations

To be updated.

## Design Optimization

To be updated.

## Design & Manufacturing

Custom parts (3D printed): From the design, the yoke, turntable, panel tray frame, and the base enclosure with a lid. Everything else is purchased from multiple sites and locations.

**Approximate budget for the design:**


| Item | Target (AED) |
|---|---|
| 2 solar panels | 80 |
| Battery cells, holder, 2S charger and protection | 100 |
| Microcontroller, LCD, LDRs, current and temperature sensors | 150 |
| 2 servos | 80 |
| Printing and laser-cutting material | 80 |
| Converter, fuse, switch, wiring | 60 |
| Reserve | 250 |
| **Total** | **800** |

## Testing and Experimental Validation

To be updated.

## Safety and Risk Register


| Risk | Control |
|---|---|
| Lithium-ion battery overheating or overcharge in desert heat | 2S protection circuit, temperature sensor with charge cutoff above 45 degrees C, shaded and ventilated enclosure |
| Short circuit | Fuse, wiring checked before power-up |
| Pinch points on the turntable and tilt mechanism | Keep hands clear while powered, emergency disconnect |
| Wind damage | Park the panels flat, test only in low wind |
| Hot surfaces and sun exposure | Marked test area, shade for the team |
| Dust ingress into electronics | Closed enclosure and lid, cable entries sealed |
| Drone-related hazard | No flight; battery pack or dummy load only |

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
