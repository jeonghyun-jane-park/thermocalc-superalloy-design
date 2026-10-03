# Revision notes - MCEN90014 Thermo-Calc report

This Overleaf-ready revision was written specifically around Kenneth Tam's annotations in the marked report.

## Annotation-by-annotation changes

- **"Very short introduction"** -> Replaced the single short introduction with a three-part technical introduction covering turbine application, gamma/gamma-prime strengthening, heat-treatment logic, CALPHAD role, and study objectives.
- **"Gap?"** -> Reworked the figure and section flow so figures follow their first in-text reference and do not create large blank pages.
- **"Missing key details" (methodology)** -> Added a calculation-plan table, composition basis, fixed processing conditions, phase-label interpretation, property equations, normalization method, mass-fraction treatment for Q4, and an explicit equilibrium-vs-kinetics limitation.
- **"Figure should appear after first in-text reference"** -> All figures are introduced in the prose before they appear; critical figures use controlled placement.
- **"Not an appropriate temperature range" / "Why not combine this with the previous figure?"** -> Combined the 700-1200 C and 400-900 C calculations into one two-panel figure, explaining what each range resolves.
- **"No analysis of third phase"** -> Added discussion of the low-temperature CRNI2_OP6 phase and why it constrains interpretation of lower ageing temperatures.
- **"Only one temperature considered"** -> Q2 now leads with the full Al-temperature phase map and uses the 800 C sweep only as the quantitative section at the prescribed ageing temperature.
- **"Omitted data"** -> Moved the complete Q3 candidate table into the Q3 section before the optimization conclusion.
- **"Why is Q3 being answered in this section?"** -> Reorganized Results by assignment question (Q1-Q5), so Q2 phase stability and Q3 multi-objective optimization are distinct.
- **"Approximately is not appropriate"** -> Replaced "approximately 7 wt%" with the supported sampled bracket: 6.89 wt% is the last sampled no-B2 point and 7.00 wt% contains BCC_B2.
- **"Q2 was partially answered ... and informs Q3"** -> The new Q2 conclusion explicitly establishes the phase-stability constraint before Q3 begins.
- **"Insufficient number of data points"** -> The report no longer calls 4 wt% a continuous/global optimum. It is explicitly the **best sampled composition**; the limitations section states that a finer Thermo-Calc sweep around 4-5 wt% is required for a continuous optimum.
- **"No given temperature" (Q4)** -> Q4 is explicitly defined and captioned at 800 C throughout.
- **"Missing key results"** -> Added an abstract and a final key-results table containing the 1050 C phase state, 800 C base strengthening, B2 onset bracket, Q3 result, Q4 result, and density implication.

## One issue that still needs original simulation metadata

The supplied files do not state the exact **Thermo-Calc software version and thermodynamic database name/version**. Those should be added to the methodology if this is intended as a fully reproducible computational report. They were not invented in this revision.

## Technical correction added

The original density section used a direct mass-fraction-weighted average of elemental densities. Because the compositions are specified by mass fraction, this revision uses the ideal additive-volume relation:

`1/rho_mix = sum(w_i/rho_i)`

This changes the comparative density estimates to approximately 7.98, 7.88, and 7.66 g/cm^3 for the base, Q3, and Q4 compositions, respectively.
