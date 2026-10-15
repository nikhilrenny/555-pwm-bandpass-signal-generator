# Marker feedback

**Module:** SEF515 Electronic Circuits, Solent University — AE1 Laboratory Report (40% weighting)
**Result:** **83 / 100** (first-class band, 74–100: "detailed design and simulation plots, and pictures of the bread-boarded full circuit and oscilloscope screenshots; analyses the design and compares measurements with theoretical or simulation results")

## Tutor comments

> This is a strong end-to-end engineering submission demonstrating clear progression from system design through simulation to hardware validation. The architecture is well structured, with particularly strong practical implementation in PWM generation and experimental verification. The main limitation is the mismatch between intended and achieved filter performance, with some corrective actions applied empirically rather than through full analytical re-derivation and optimisation.

### Strengths
- Solid system-level design: clear PWM → filter → amplification signal chain with correct functional decomposition
- Strong PWM implementation: correct derivation, stable duty-cycle control (~17% consistently achieved)
- Good experimental methodology: oscilloscope measurements, frequency sweeps, RMS/Vpp extraction
- Strong simulation workflow: transient + AC sweep + Bode analysis used effectively
- Good real-world engineering awareness: tolerance effects, GBW limits, parasitics correctly identified
- Proper use of buffering and impedance isolation between stages
- Clear comparison across theory, simulation, and hardware results

### Improvements
- The filter stage does not meet design specifications (centre frequency and bandwidth significantly drift in hardware)
- Filter synthesis lacks full analytical rigour (no complete transfer function/pole derivation tied to the −40 dB requirement)
- Design corrections are empirical (component "fixes") rather than re-optimised from first principles
- No formal sensitivity/tolerance analysis during the design phase (only discussed after failure)
- Limited quantitative proof of specification compliance at the system level
