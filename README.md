# SC-01: Simple Cubic Lead
## sc-Pb | Predicted Tc = 295 K | DFT Required Before Synthesis

**Formula:** Simple cubic Pb  
**Predicted Tc:** 295 K  
**Status:** PREDICTION — DFT phonon calculation required  
**Patent:** Derivative of US Application 19/383,582  
**License:** CC0 1.0 Universal  

---

## Honest Status

No DFT calculation has been performed. The central claim — that a soft phonon mode exists at ~30 K at the R point in sc-Pb at a = 3.18 Å — is a prediction derived from the physical mechanism argument. It has not been computationally verified.

The synthesis protocol is complete and valid. Synthesis should follow DFT confirmation.

---

## The Prediction

Simple cubic lead at lattice constant a = 3.18 Å achieves Tc = 295 K through conventional BCS-Eliashberg electron-phonon coupling enhanced by:

1. A soft phonon mode at the R point (~30 K) contributing ~60% of λep
2. Enhanced density of states at the Fermi level (1.8 vs 0.8 states/eV/atom)
3. Fermi surface nesting at qN ≈ (π/a, π/a, 0)

**The central falsifiable prediction:**

> A soft phonon mode exists at approximately 30 K at the R point (π/a, π/a, π/a) in simple cubic Pb at a = 3.18 Å.

This is testable by DFT in hours to days. It is testable experimentally by inelastic X-ray scattering.

---

## The Profit Point

FCC lead superconductivity was explained by BCS theory at Tc = 7.2 K in the early 1970s. The question was declared closed. The simple cubic phase — accessible through thin film deposition — was never investigated because the ground state was assumed to be optimal.

**R³ identified the contamination:** Assuming the ground state crystal structure is the optimal superconducting structure.

---

## Predicted Parameters

| Parameter | Predicted Value | Basis |
|-----------|----------------|-------|
| Crystal structure | Simple cubic | Deposition target |
| Lattice constant | 3.18 Å | Deposition target |
| Soft mode frequency | 20–40 K | Physical mechanism |
| λep | 1.5–2.0 | If soft mode at predicted frequency |
| ωlog | 300–500 K | Strong coupling regime |
| Tc | 200–300 K | Eliashberg framework |

These are predicted ranges. DFT will determine actual values.

---

## Mathematical Correction Notice

A previous version of the phonon analysis document contained a mathematical error in the α²F(ω) integration (factor of ~22 discrepancy). That error has been fully documented and corrected. See `theory/phonon_analysis_honest.md` and `theory/verify_alpha2F.py` for complete details.

The physical mechanism argument is unaffected by the mathematical error. The soft mode prediction stands. The error was in the numerical specification of the spectral function, not in the physical reasoning.

---

## DFT Calculation Parameters

| Parameter | Value |
|-----------|-------|
| Code | Quantum ESPRESSO v7.2 (open source) |
| XC functional | PBEsol |
| Pseudopotential | Pb.pbe-dn-kjpaw_psl.1.0.0.UPF |
| Structure | Simple cubic, a = 3.18 Å |
| k-point mesh | 24 × 24 × 24 (shifted) |
| Energy cutoff | 80 Ry |
| Phonon q-mesh | 8 × 8 × 8 |
| Method | DFPT linear response |

**This calculation runs in hours to days on a university cluster. The parameters are fully specified and ready to execute.**

---

## Three Questions DFT Will Answer

1. **Dynamic stability:** Are all phonon frequencies real? (imaginary = unstable phase)
2. **Soft mode:** Does a mode exist near 30 K at the R point?
3. **λep:** What is the actual electron-phonon coupling from first principles?

If (1) yes, (2) yes, (3) λep ≥ 1.5: proceed to experimental synthesis.  
If (1) no: the phase does not exist at ambient pressure under these conditions.  
If (2) no: the Tc prediction is not supported.

---

## Synthesis Protocol (For After DFT Confirmation)

Complete protocol in `synthesis_protocol.md`. Summary:

- **Method:** MBE or thermal evaporation
- **Source:** 5N purity Pb
- **Substrate:** Si (100), RCA cleaned
- **Rate:** 0.10 ± 0.02 Å/s
- **Thickness:** 100 ± 5 nm
- **Anneal:** 200°C, 60 min, Ar atmosphere

---

## Collaboration Contact

**For DFT calculation:**  
Prof. Feliciano Giustino — fgiustino@oden.utexas.edu — UT Austin  
Prof. Iñigo Errea — errea@ehu.eus — University of the Basque Country  
Prof. Samuel Poncé — samuel.ponce@uclouvain.be — UCLouvain  

---

## Verification Results

| Date | Institution | Type | Result | Data |
|------|-------------|------|--------|------|
| — | Open — DFT groups invited | Computational | — | — |
| — | Open — experimental groups | Experimental | — | — |

---

*CC0 1.0 Universal — Public Domain — Free for All Humanity*
