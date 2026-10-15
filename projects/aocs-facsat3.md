# CubeSat B-dot / ADCS — Simulation and Engineering Case Study
**Sofía Hurtado Ramos · Mechatronics engineering · V2**

An academic demonstrator for reducing a CubeSat's angular rate after deployment, developed in MATLAB/Simulink and presented through an interactive technical review website.

## Engineering work
- Model-based magnetic detumbling control and sensor/actuator timing.
- A stratified Monte Carlo campaign with recorded seeds and acceptance criteria.
- Separate fault detection, isolation and recovery (FDIR) tests.
- Translation of six stakeholder needs into eleven engineering metrics through QFD.
- A catalogue of 56 candidate failure modes and explicit verification gaps.
- Preliminary hardware comparisons and an 18-month design/build/integration schedule.

## Results and what they mean
| Evidence | Result | Interpretation |
|---|---|---|
| Main control campaign | 922 PASS / 1,000 runs | Demonstrator criteria, not mission reliability. |
| Initial angular-rate groups | 334 at 5 °/s, 333 at 10 °/s, 333 at 30 °/s | All 78 FAIL cases belong to the 30 °/s group. |
| Separate FDIR tests | Nine test contracts passed, including one healthy case | Does not establish coverage of all candidate failure modes. |
| Forced-output fault | Current persisted despite logical inhibition | Motivates independent physical power isolation. |
| QFD | Six needs, eleven metrics, weighted total 1,076 | Engineering priorities, not supplier certification or percent compliance. |

## Decisions informed by the analysis
1. Review actuator authority and model assumptions for the high-rate group rather than assuming that a larger magnetorquer solves every failure.
2. Distinguish command limits from physical electrical and thermal ratings.
3. Include an independent power-cut architecture and verify residual current.
4. Size the power system using total spacecraft loads; copper-loss energy alone is insufficient.
5. Treat commercial parts as candidates pending interface, thermal, mechanical and supplier verification.

## Implementation planning
The proposal covers design, construction, integration and testing of a 1U CubeSat with a project mass ceiling of 3 kg. Packing, deployer compatibility, mass margin and inertia remain to be closed. Architectural scalability toward a 100–150 kg microsatellite is a study criterion, not a demonstrated capability.

## Portfolio evidence
- [Interactive technical portfolio](https://sofiahurtadoramos-aocs-facsat3.lovable.app)
- Detailed scripts, protocols, results and implementation workbooks are maintained in the private project repository. Access can be arranged for technical review.

## Scope
Simulation and engineering preparation only: no flight hardware qualification, launch readiness or NASA certification is claimed. Selected NASA practices informed documentary traceability and gap analysis. This work does not imply employment by a space agency or access to confidential mission data.
