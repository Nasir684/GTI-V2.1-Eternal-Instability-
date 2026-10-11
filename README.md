# GTI v2.1 — Eternal Instability: Stability as the Limit of Finite Dwell Times

**One testable signature. No regulator, no stabilizing field.**

> Stability is not a property of states but the n→∞ limit of finite dwell times in a bounded potential, diverging because escape saddles widen (W_n ∝ n^{β/2}), not because barriers deepen.

**Author:** Nasir Khan — nasirk684@gmail.com — ORCID: 0009-0002-6006-0796
**Version:** v2.1 — 12 Oct 2026
**Status:** Active — Falsifiable
**Predecessor:** GTI v1 — Withdrawn — M_stab 10³ → O(1) wrong sign. See Sec 2.4 autopsy. Link: https://github.com/yourname/GTI-v1-withdrawn

---

### Abstract
Bounded C² potential on ℝ with infinite degenerate wells V(a_n)=v₀, spacing L_n=λW_n, saddles same height h=v₀+ΔV but width scheduled V(s_n+u)=h-ΔV φ(u/W_n), W_n=W₀n^{β/2}. Curvature derived κ_n=ΔV φ''(0)/W_n². Dynamics overdamped Langevin dX=-V'dt+g dW, g≥g₀>0 inevitable. Bounded → no normalizable stationary density → null recurrent washboard → stability only conditional MFPT. Exact: τ_n=τ₀W_n, τ₀=(2√π/gω₀)e^{2ΔV/g²} I_φ(2ΔV/g²). Ratio law τ_{n+1}/τ_n=(1+1/n)^{β/2} exact parameter-free. Slope logτ=-½logκ at fixed ΔU, κ independently via T_cr,n=ħ√(κ_n/m)/2πk_B.

### What Changed From v1
v1: M_stab regulator, 10³ suppression claimed, barrier deepening implied, LIGO echo predicted
v2.1: No regulator — suppression replaced by waiting, bounded potential no barrier can deepen, LIGO predictions withdrawn pending independent V_eff, hierarchy exact not estimated

### LIGO Closure Statement
Consequently, GTI v2.1 makes no testable prediction for LIGO O4/O5 or echo searches without an independently derived V_eff for merger remnant. The white-hole/echo chapter from v1 is closed pending such derivation. v1's 10³ suppression claim is formally withdrawn.

### Testbed: Josephson Circuits
Single junction: M=(ħ/2e)²C, U(φ)=-E_J(cosφ+sφ), s=I/I_c. At I_c=1μA C=1pF s=0.95: ω_p/2π=4.9GHz ΔU/k_B=0.50K T_cr=37mK.

Mapping: X↔φ√M, ω₀²↔ω_p², W↔Δφ_s√M, g²↔2k_BT.

Protocol A — C-sweep at fixed bias (I_c,s fixed): logτ=½logC vs logC, -½ vs logκ, T_cr∝C^{-1/2} 53→19mK. C={0.5,1,2,4}pF factor 8 in κ.

Protocol B — Matched-barrier bias leverage: κ=ΔU·r(s)/M r(s)=√(1-s²)/(2g(s)) r≈3/(4(1-s)) 7.3→750 at s=0.9→0.999 two decades κ at fixed barrier via scaling E_J.

Measurement: switching histograms P(I_sw)→Γ(I). Existing archives re-analyzable.

### Falsifiers
F1: Demonstration of decay-proof state Γ≡0 with no escape channel — kills P1.
F2: Failure of slope -½ at matched ΔU beyond Q-dispersion systematic across independent ensembles, or pointwise failure of ratio law in multiwell device.

### Repository Structure
paper/gti_v2.1.pdf — final PDF
paper/gti_v2.1.tex — TeX source
src/mfpt_derivation.py — checks τ_n=τ₀W_n and ratio law
src/langevin_sim.py — optional 10-well Langevin demo
figures/ — W ladder, ratio law, Josephson protocol

### Reproducibility
python src/mfpt_derivation.py
python src/langevin_sim.py

### Postulates Cost
P1+P2 → no stationary density → stability only conditional dwell Sec 2.3
P2 → no g→0 limit → kick inevitable
P3 → stability = MFPT with reflecting boundary — null recurrence forces conditional

### Citation
GTI v2.1 — Eternal Instability (2026) https://github.com/yourname/GTI-v2.1-eternal-instability

### License
Paper: CC-BY-4.0 Code: MIT
Topics: metastability kramers-escape josephson-junction null-recurrence falsifiable-theory
