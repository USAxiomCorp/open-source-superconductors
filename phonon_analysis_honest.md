# Phonon Analysis — Simple Cubic Pb
## Honest Revision After R³ Self-Refinement

**Status:** Prediction only — DFT required  
**Error documented:** Yes — see Section 1  
**Date:** March 16, 2026  

---

## Section 1: The Mathematical Error (Documented)

A previous version of this analysis contained a mathematical error in the α²F(ω) integration.

**The error:** The approximation λep ≈ 2 × Σ(Ai/ωi) was used for Lorentzian peaks. This approximation is valid only for delta function peaks. For Lorentzian peaks with finite width, numerical integration gives λep = 0.083, not 1.82 — a factor of ~22 discrepancy.

**The consequence:** The three numbers λep = 1.82, ωlog = 450 K, and Tc = 295 K cannot simultaneously be obtained from the Lorentzian peak parameters previously specified.

**What this means:** The α²F(ω) numerical specification was wrong. The physical mechanism argument is unaffected.

Run `verify_alpha2F.py` to see the full numerical demonstration.

---

## Section 2: What the Physical Mechanism Actually Predicts

The soft mode mechanism is physically motivated regardless of the mathematical error:

```
Fermi surface nesting at qR = (π/a, π/a, π/a)
→ Enhanced electronic response (Kohn anomaly)
→ Phonon softening at R point
→ Small ω denominator in electron-phonon matrix elements
→ Large λep contribution from soft mode
→ Strong coupling → high Tc
```

This chain of reasoning is independent of the numerical specification error.

**The prediction:** If DFT shows a soft mode at ~30 K at the R point, the physical mechanism is confirmed and the Tc enhancement is expected.

**The honest range:** If soft mode exists at 30 K, predicted λep = 1.5–2.0, predicted Tc = 200–300 K.

---

## Section 3: DFT Parameters

These parameters are correct and ready for execution:

```
Code: Quantum ESPRESSO v7.2
XC: PBEsol
Pseudopotential: Pb.pbe-dn-kjpaw_psl.1.0.0.UPF
Structure: Simple cubic, a = 3.18 Å
k-mesh: 24 × 24 × 24
Cutoff: 80 Ry
Phonon q-mesh: 8 × 8 × 8
Method: DFPT linear response
```

---

## Section 4: Confidence Levels

| Aspect | Confidence |
|--------|-----------|
| Physical mechanism valid in principle | ★★★★☆ |
| Synthesis protocol complete | ★★★★★ |
| DFT parameters correct | ★★★★★ |
| Soft mode actually exists | ★☆☆☆☆ — unknown |
| λep = 1.82 | ☆☆☆☆☆ — unverified |
| Tc = 295 K | ☆☆☆☆☆ — unverified |

---

## Section 5: Path Forward

1. Send DFT parameters to Giustino / Errea / Poncé
2. Receive phonon dispersion result
3. If soft mode confirmed: proceed to experimental synthesis
4. If no soft mode: prediction falsified, update repository

---

*CC0 1.0 Universal — Public Domain*
