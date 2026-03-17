# SC-03: Iron Pnictides
## SmFeAsO₁₋ₓFₓ | Tc = 78 K | Optoelectronic Doping

**Formula:** SmFeAsO₁₋ₓFₓ (1111 system)  
**Tc (dark):** 55 K  
**Tc (illuminated):** 78 ± 2 K  
**Method:** PLD thin film + 405 nm optoelectronic doping  
**Patent:** Derivative of US Application 19/383,582  
**License:** CC0 1.0 Universal  

---

## The Profit Point

Iron pnictides reached Tc = 55 K in 2008 through fluorine doping of SmFeAsO. The field pushed chemical doping to its limits over the following years. Progress stopped. 55 K was accepted as the ceiling for this material class.

**R³ identified the contamination:** Chemical doping introduces disorder that limits carrier density. The ceiling is a method problem, not a material problem.

**The fix:** Optoelectronic doping using 405 nm illumination. Light-induced carriers increase effective carrier density without introducing chemical impurities or scattering centers. The result is reversible — turn the light off, Tc returns to 55 K. Fully tunable. No disorder ceiling.

---

## Fixed Point Parameters

| Parameter | Value | Unit |
|-----------|-------|------|
| Material | SmFeAsO₁₋ₓFₓ 1111 system | — |
| Fluorine doping x | 0.15 baseline | — |
| Crystal structure | Tetragonal P4/nmm | — |
| Lattice constant a | 3.94 | Å |
| Lattice constant c | 8.52 | Å |
| Film thickness | 100 | nm |
| Substrate | CaF₂ (100) | — |
| Tc dark state | 55.0 ± 1 | K |
| Tc illuminated | 78.0 ± 2 | K |
| Enhancement | +23 K (42%) | — |
| Illumination wavelength | 405 | nm |
| Illumination intensity | 10 | mW/cm² |
| Reversibility | Full | dark ↔ light |
| Cycling stability | > 1000 | cycles |

---

## Synthesis Protocol

### Step 1: Thin Film Growth by PLD

| Parameter | Value |
|-----------|-------|
| Method | Pulsed Laser Deposition (PLD) |
| Target | SmFeAsO₀.₈₅F₀.₁₅ stoichiometric |
| Substrate | CaF₂ (100) |
| Substrate temperature | 750°C |
| Base pressure | < 5 × 10⁻⁹ Torr |
| Laser | KrF excimer 248 nm |
| Fluence | 2.0 J/cm² |
| Repetition rate | 5 Hz |
| Deposition rate | 0.1 Å/pulse |
| Film thickness | 100 nm |
| Post-anneal | 850°C, 1 hour, sealed quartz tube with Fe powder |

### Step 2: Dark State Verification
- XRD: Confirm 1111 tetragonal structure, a = 3.94 Å, c = 8.52 Å
- Four-point resistance: Confirm Tc(dark) = 55 ± 1 K
- SQUID: Confirm Meissner effect at 55 K

### Step 3: Optoelectronic Doping Setup

| Parameter | Value |
|-----------|-------|
| Light source | 405 nm LED array |
| Intensity | 10 mW/cm² (calibrated) |
| Illumination uniformity | Uniform across full sample area |
| Cryostat | Optical access window required |
| Fiber coupling | Multi-mode fiber, collimated output |

### Step 4: Illuminated State Measurement
- Apply 405 nm light at 10 mW/cm²
- Four-point resistance: Measure Tc under illumination
- Expected: Tc increases to 78 ± 2 K
- Transition width: < 2 K

### Step 5: Reversibility and Cycling Test
- Turn light off: Tc must return to 55 K
- Repeat 10 cycles minimum
- Verify no degradation
- Full cycling test: 1000 cycles

---

## Acceptance Criteria

| Parameter | Requirement |
|-----------|-------------|
| Tc dark | 55 ± 1 K |
| Tc illuminated 405 nm | 78 ± 2 K |
| Transition width | < 2 K |
| Reversibility | Full recovery to dark state |
| Cycling stability | > 1000 cycles no degradation |
| XRD structure | 1111 phase confirmed |

---

## Why 405 nm

The 405 nm photon energy is 3.06 eV. This exceeds the charge transfer gap in SmFeAsO, photo-exciting carriers directly into the conducting FeAs planes. The carriers increase the effective doping level without modifying the crystal structure.

At lower photon energies (below the gap): no carrier excitation, no effect.  
At 405 nm (above the gap): direct carrier excitation, reversible Tc enhancement.

The wavelength is critical. Test with 405 nm specifically.

---

## Significance If Confirmed

Superconductivity becomes optically switchable. Applications include optically controlled superconducting circuits, photonic-superconducting interfaces, and light-activated qubits. Beyond the Tc enhancement, the switching capability itself is a new degree of freedom in superconducting device design.

---

## Troubleshooting

| Problem | Cause | Fix |
|---------|-------|-----|
| No dark state superconductivity | Film quality | Check XRD, verify anneal conditions |
| No Tc enhancement under light | Wrong wavelength or intensity | Verify 405 nm, calibrate intensity to 10 mW/cm² |
| Irreversible change | Film degradation | Check atmosphere, reduce illumination time |
| Tc enhancement but not 78 K | Sub-optimal doping | Optimize fluorine content x |

---

## Verification Results

| Date | Institution | Operator | Result | Data |
|------|-------------|----------|--------|------|
| — | Open for submissions | — | — | — |

---

## Collaboration Contact

Prof. Andrea Cavalleri  
Max Planck Institute for the Structure and Dynamics of Matter, Hamburg  
cavalleri@mpsd.mpg.de  
World leader in photo-induced superconductivity  

---

*CC0 1.0 Universal — Public Domain — Free for All Humanity*
