# SC-01: Synthesis Protocol
## Simple Cubic Lead — For Use After DFT Confirmation

**Status:** Complete protocol — execute after DFT confirms soft mode  
**Material:** sc-Pb, a = 3.18 Å  
**Method:** MBE or thermal evaporation  

---

## Prerequisites

Do not attempt synthesis until DFT calculation confirms:
1. Dynamic stability of sc-Pb at a = 3.18 Å (all real phonon frequencies)
2. Soft mode present near 30 K at R point
3. λep ≥ 1.5 from first principles

---

## Materials

| Item | Specification | Supplier |
|------|--------------|---------|
| Lead source | ≥ 99.999% (5N) purity, granules or shot | Alfa Aesar #10285 or equivalent |
| Substrate | Si (100), 10×10 to 25×25 mm, polished | UniversityWafer Si-100-P-1 or equiv |
| Argon gas | 99.999% | For annealing atmosphere |
| Acetone | Semiconductor grade | Substrate cleaning |
| Isopropanol | Semiconductor grade | Substrate cleaning |
| DI water | 18.2 MΩ·cm | All rinsing |

---

## Equipment

| Equipment | Specification |
|-----------|--------------|
| Deposition system | MBE (base ≤ 5×10⁻¹⁰ Torr) or thermal evap (≤ 5×10⁻⁷ Torr) |
| Rate monitor | Quartz crystal microbalance, ±0.01 Å/s |
| Annealing furnace | Programmable, ±1°C, inert atmosphere |
| XRD | Cu Kα, 2θ range 20–80°, step ≤ 0.02° |
| Four-point probe | With cryostat 250–310 K range |
| SQUID magnetometer | Sensitivity ≤ 10⁻⁸ emu |

---

## Procedure

### Step 1: Substrate Preparation (RCA Clean)

1. Degrease in acetone, 5 min ultrasonic
2. Rinse in isopropanol, 5 min ultrasonic
3. Rinse in DI water
4. SC1: NH₄OH:H₂O₂:H₂O (1:1:5) at 75°C, 10 min
5. Rinse DI water, 5 cycles
6. SC2: HCl:H₂O₂:H₂O (1:1:6) at 75°C, 10 min
7. Rinse DI water, 10 cycles
8. Blow dry with N₂
9. Load into deposition chamber immediately

### Step 2: System Preparation

1. Load 5N Pb source (0.5–1.0 g)
2. Mount substrate on manipulator
3. Pump to base pressure (≤ 5×10⁻⁷ Torr minimum)
4. Calibrate QCM rate monitor

### Step 3: Deposition

| Parameter | Value |
|-----------|-------|
| Substrate temperature | Room temperature (20–25°C) |
| Deposition rate | 0.10 ± 0.02 Å/s |
| Target thickness | 100 ± 5 nm |
| Chamber pressure | ≤ 5×10⁻⁷ Torr during deposition |

1. Stabilize source temperature (30 min equilibration)
2. Open shutter, begin deposition at 0.10 Å/s
3. Monitor thickness via QCM
4. Close shutter at 100 nm target

### Step 4: Annealing

1. Transfer to annealing furnace
2. Purge with Ar (99.999%) at 1 L/min
3. Ramp at 10°C/min to 200°C
4. Hold at 200°C for 60 minutes
5. Cool at 5°C/min to room temperature
6. Maintain Ar atmosphere throughout
7. Store in vacuum or N₂ immediately

---

## Characterization

### XRD (Structure Verification)

Scan 2θ = 20–80°, step 0.02°, 1°/min

**Expected peaks for simple cubic phase:**

| (hkl) | 2θ (calculated) | Intensity |
|-------|----------------|-----------|
| (100) | 29.2° | Weak |
| (110) | 41.8° | Strong |
| (111) | 52.1° | Medium |
| (200) | 60.7° | Medium |
| (211) | 77.5° | Weak |

Expected lattice constant: a = 3.180 ± 0.005 Å

**If FCC peaks appear instead:** Annealing did not produce simple cubic phase. Optimize annealing protocol.

### Four-Point Resistance

- Measure resistance 270–310 K in 0.1 K steps near expected Tc
- Tc defined as temperature at 50% of normal-state resistance

### SQUID Magnetometry

- ZFC/FC protocol
- Cool to 250 K in zero field
- Apply 10 Oe measuring field
- Warm from 250 K to 310 K recording χ(T)
- Cool from 310 K to 250 K in field recording χ(T)

---

## Acceptance Criteria

| Parameter | Requirement |
|-----------|-------------|
| XRD: crystal structure | Simple cubic, a = 3.180 ± 0.005 Å |
| XRD: phase purity | > 90% sc-Pb |
| Resistance: Tc | 295 ± 2 K |
| Resistance: zero resistance | Below noise floor |
| SQUID: Meissner effect | χ < −0.1 (SI) |
| SQUID: Tc onset | 295 ± 2 K |

---

## Troubleshooting

| Problem | Cause | Fix |
|---------|-------|-----|
| No transition observed | Wrong phase (FCC) | Check XRD, optimize anneal |
| FCC phase in XRD | Annealing insufficient | Increase anneal time or temperature |
| Transition outside 295±2 K | Lattice constant off | Verify deposition rate, check XRD |
| Broad transition (>5 K) | Film non-uniform | Use rotating substrate holder |

---

## Safety

Lead is a toxic heavy metal. Use PPE (gloves, lab coat, eye protection). Work in fume hood. Dispose as hazardous waste. Wash hands thoroughly after handling.

---

*CC0 1.0 Universal — Public Domain — Free for All Humanity*
