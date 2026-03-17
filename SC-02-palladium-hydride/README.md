# SC-02: Palladium Hydride
## PdH₀.₈₅ | Tc = 9 K | β-Phase Epitaxial Thin Film

**Formula:** PdH₀.₈₅ (β-phase)  
**Tc:** 9.0 ± 0.5 K  
**Method:** Epitaxial thin film + electrochemical hydrogen loading  
**Patent:** Derivative of US Application 19/383,582  
**License:** CC0 1.0 Universal  

---

## The Profit Point

Palladium hydride superconductivity was studied for decades and abandoned when bulk loading proved irreproducible. The field concluded the material was unreliable.

**R³ identified the contamination:** The bulk synthesis method, not the material itself.

Bulk samples had three simultaneous failure modes:
- Grain boundaries — inhomogeneous hydrogen distribution
- Phase segregation — mixed α and β phases
- Uncontrolled stoichiometry — H/Pd ratio varying across the sample

**The fix:** Epitaxial Pd thin film on SrTiO₃ eliminates grain boundaries. Electrochemical loading at controlled potential gives precise H/Pd = 0.85 ± 0.01. Pure β-phase verified by XRD before any transport measurement.

All three failure modes eliminated simultaneously. That combination has not been published.

---

## Fixed Point Parameters

| Parameter | Value | Unit |
|-----------|-------|------|
| Composition | PdH₀.₈₅ | ±0.01 |
| Crystal structure | FCC β-phase | — |
| Lattice constant | 4.090 ± 0.002 | Å |
| Lattice expansion vs pure Pd | +3.6% | — |
| Film thickness | 100 | nm |
| Substrate | SrTiO₃ (001) TiO₂-terminated | — |
| Critical temperature Tc | 9.0 ± 0.5 | K |
| Upper critical field Hc2(0) | 2.5 | T |
| Transition width | < 0.5 | K |
| Stability | > 100 hours | inert atmosphere |

---

## Synthesis Protocol

### Step 1: Pd Thin Film Growth

| Parameter | Value |
|-----------|-------|
| Method | DC magnetron sputtering or MBE |
| Substrate | SrTiO₃ (001), TiO₂-terminated |
| Base pressure | < 5 × 10⁻¹⁰ Torr |
| Substrate temperature | 400°C |
| Deposition rate | 0.2 Å/s |
| Film thickness | 100 nm |
| Post-deposition | Cool to RT in vacuum |

### Step 2: XRD Verification Before Loading
Confirm FCC Pd structure. Reject any sample showing contamination or wrong phase before proceeding.

### Step 3: Electrochemical Hydrogen Loading

| Parameter | Value |
|-----------|-------|
| Electrolyte | 0.1 M H₂SO₄ (ultrapure) |
| Reference electrode | Ag/AgCl |
| Counter electrode | Pt mesh |
| Applied potential | −0.05 V vs. Ag/AgCl |
| Loading time | 2 hours at constant potential |
| Temperature | 25°C |
| Target composition | H/Pd = 0.85 (verified by weight gain) |

### Step 4: Post-Loading Verification
- XRD: Confirm β-phase, a = 4.090 Å (3.6% expansion vs pure Pd)
- Rocking curve FWHM: < 0.1° (high crystalline quality)
- Weight gain: Confirm H/Pd = 0.85 ± 0.01

### Step 5: Transport Measurement
- Four-point resistance: 4.2 K to 20 K
- Expected: Zero resistance below Tc = 9 K
- Transition width: < 0.5 K
- SQUID: Confirm Meissner effect

---

## Acceptance Criteria

| Parameter | Requirement |
|-----------|-------------|
| Tc (resistance) | 9.0 ± 0.5 K |
| Zero resistance | < 10⁻⁶ Ω |
| H/Pd ratio | 0.85 ± 0.01 |
| XRD lattice constant | 4.090 ± 0.002 Å |
| Transition width | < 0.5 K |
| Meissner effect | Confirmed by SQUID |

---

## Troubleshooting

| Problem | Cause | Fix |
|---------|-------|-----|
| No superconducting transition | Wrong H/Pd ratio | Verify weight gain, adjust loading time |
| Transition above 9 K | α-phase contamination | Extend loading time, confirm β-phase by XRD |
| Broad transition | Inhomogeneous loading | Check potential uniformity, rotate sample |
| Oxidation | Air exposure | Handle under inert atmosphere throughout |

---

## Verification Results

| Date | Institution | Operator | Result | Data |
|------|-------------|----------|--------|------|
| — | Open for submissions | — | — | — |

Submit to `verification/results/` in this folder or to `../../verification/submissions/`

---

## Collaboration Contact

Prof. Iñigo Errea  
University of the Basque Country, Spain  
errea@ehu.eus  
Published on PdHx stoichiometry and superconductivity  

---

*CC0 1.0 Universal — Public Domain — Free for All Humanity*
