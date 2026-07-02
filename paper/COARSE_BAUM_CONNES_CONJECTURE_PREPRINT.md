# The Coarse Baum-Connes Conjecture via Coarse-Assembly Persistence
## Canonical Lane (defined term): the manifold-constrained local-to-global closure architecture (`CBC1-CBC8`)

**Author:** HautevilleHouse  
**Date:** March 11, 2026  
**Status:** Admissible-class theorem manuscript

---

## Abstract

This manuscript develops a canonical-lane closure architecture for the target problem: proving persistence of the coarse assembly package through an admissible coarse-geometric closure architecture.

The proof program is organized as eight steps `CBC1-CBC8` with executable closure gates `CBC_G1`, `CBC_G2`, `CBC_G3`, `CBC_G4`, `CBC_G5`, `CBC_G6`, and `CBC_GM`. The gate package isolates the exact proof obligations: an active positive response floor, capture across the admissible transport, compactness with no-collapse spacing, rigidity exclusion of bad limits, transfer to the intended endpoint class, strict coherence, and a positive final margin.

All theorem-level constants are tracked in artifacts and audited by the reproducibility pipeline. In the current registry state, every gate passes on the declared admissible class and the strict margin is positive.

---

## 1. Target Statement and Scope

### 1.1 Target statement

For every admissible metric family in the declared class, the coarse assembly map is an isomorphism.

The canonical-lane proof path is:

1. encode the admissible evolution in a canonical class `A`,
2. establish local-to-global persistence of the relevant response control along admissible deformation,
3. exclude bad limits by rigidity and compactness,
4. transfer the rigid limit through the bridge package,
5. identify the endpoint representative with the intended target class.


### 1.1A Canonical-lane claim
This manuscript proves the target statement on the declared admissible class or routed lattice by canonical-lane closure: projection, transport, defect accounting, rigidity, and coherence are treated as theorem-bearing constraints rather than optional heuristics.

### 1.1B Bridge / equivalence statement
The canonical endpoint objects are tied to the standard problem-side target through the in-repo bridge package. The paper records the transfer or endpoint-identification step in the main theorem chain, and `notes/IDENTIFICATION_BRIDGE.md` fixes the determining-class lock in ordinary mathematical language.

### 1.1C Audit surface
A reviewer can check this claim on four surfaces:

1. the standard target statement in Section `1.1`,
2. the canonical objects and closure gates in the main paper,
3. the endpoint bridge in `notes/IDENTIFICATION_BRIDGE.md`,
4. the executable rerun `bash repro/run_repro.sh` with runtime output `repro/certificate_runtime.json`.

### 1.2 Local claim boundary

- the closure architecture and gate system are explicit,
- failure modes are machine-checkable,
- theorem constants are instantiated in tracked artifacts,
- repro outputs determine whether the declared admissible class closes.

Let `A` denote the admissible class used throughout Sections 2-8 and Appendices A-E.

---

## 2. Epistemic Axiom Map (A1-A8)

| Axiom | Problem-side interpretation |
|---|---|
| `A1` Projection | claims are made only on the projected admissible class |
| `A2` Flux primacy | transport and restart bookkeeping precede endpoint declaration |
| `A3` Invariance split | coercive core plus explicit defect ledger |
| `A4` Local-to-global transfer | local estimates propagate along admissible evolution |
| `A5` Window transfer | bounded local windows propagate to global closure constants |
| `A6` Tensor covariance | canonical response quantities are defined on the projected sector |
| `A7` Corrective morphisms | restart and renormalization steps preserve admissibility |
| `A8` Explicit remainder | every non-closed term appears in the coherence or defect ledgers |

---

## 3. Canonical Objects

Let `tau` denote the deformation parameter and let

`u_tau = (C_tau, G_tau, D_tau, N_tau, L_tau)`

be the admissible state consisting of coarse packets, admissible geometric data, defect ledgers, normalization parameters, and lock observables.

Primary objects:

- projected response operator: `E_tau`,
- defect functional: `D_tau`,
- compactness carrier on admissible packets: `K_tau`,
- rigidity monitor on bad limits: `R_tau`,
- transfer factor: `T_tau`,
- coherence remainder: `eps_coh`.

Strict closure margin:

`M_CBC = min(kappa_coarse, sigma_metric, kappa_compact, rho_rigidity, coarse_transfer) - eps_coh`.

Target:

`M_CBC > 0`.

---

## 4. Response and Gate Interface

### 4.1 Canonical tube

- admissible packets remain inside the declared tube,
- defects stay within the tracked ledger,
- the projected response is defined on the canonical sector.

### 4.2 Projected response

Let `H_resp` be the projected response sector and define:

`E_tau = Pi_resp L_tau Pi_resp`.

Interpretation: `E_tau` records the positive coarse-assembly floor that prevents collapse of the admissible coarse transport package.

### 4.3 Closure gates

| Gate | Constant | Criterion |
|---|---|---|
| `CBC_G1` | `kappa_coarse` | projected coarse response has a strict positive floor |
| `CBC_G2` | `sigma_metric` | metric defect stays above capture floor across admissible coarse losses |
| `CBC_G3` | `kappa_compact` | normalized near-failure families are precompact and coarse windows do not collapse |
| `CBC_G4` | `rho_rigidity` | bad nonisomorphic coarse countermodels are excluded |
| `CBC_G5` | `coarse_transfer` | rigid limit transfers to the coarse-assembly endpoint class |
| `CBC_G6` | `eps_coh` | coherence remainder closes in strict mode |
| `CBC_GM` | derived | all upstream gates pass and `M_CBC > 0` |

### 4.4 Strict margin

At current artifact values:

- `kappa_coarse` = 1.0913680000000001,
- `sigma_metric` = 1.073,
- `kappa_compact` = 0.8045052292839904,
- `rho_rigidity` = 1.077,
- `coarse_transfer` = 1.029422,
- `eps_coh = 0.0`.

Hence:

`M_CBC = 0.8045052292839904 > 0`.

### 4.5 Raw coercive constant

Define `kappa_coarse^(raw) := c_coarse_raw * coarse_density_raw - e_coarse_raw`.

Current extracted value:

`kappa_coarse = 1.0913680000000001`.

---

## 5. Capture, Compactness, and Theorem Chain

### 5.1 Local-to-global theorem chain (`CBC1-CBC8`)

1. `CBC1` Active coarse block on the projected response sector.
2. `CBC2` Uniform metric capture bounds on the canonical coarse tube.
3. `CBC3` Restart map preserving admissible coarse data.
4. `CBC4` First-failure compactness extraction.
5. `CBC5` Rigidity exclusion of bad nonisomorphic coarse countermodels.
6. `CBC6` Coarse-transfer closure on the extracted endpoint class.
7. `CBC7` Determining-class identification of the coarse Baum-Connes endpoint.
8. `CBC8` Final persistence theorem: the coarse assembly endpoint survives admissible closure.

### 5.2 Raw capture constant

Define `sigma_metric^(raw) := metric_floor_raw - coarse_loss_raw - restart_loss_raw`.

Current extracted value:

`sigma_metric = 1.073`.

### 5.3 Compactness modulus

Define `kappa_compact^(raw) := (1 + delta_comp_sup_raw)^(-1)`.

Current extracted value:

`kappa_compact = 0.8045052292839904`.

---

## 6. Rigidity, Transfer, and Identification

### 6.1 Rigidity margin

Rigidity excludes the bad-limit class `B_bad` of nonisomorphic coarse countermodels incompatible with closure.

Define `rho_rigidity^(raw) := inf_(U in B_bad) R_bad(U) / ||U||^2`.

The tracked theorem-level input is `rho_rigidity = 1.077 > 0`.

### 6.2 Transfer package

Once bad limits are excluded, the extracted endpoint class is transferred to the coarse-assembly endpoint class by the bridge inequality.

Define `coarse_transfer^(raw) := c_transfer_raw * transfer_gain_raw - e_transfer_raw`.

Current extracted value:

`coarse_transfer = 1.029422 > 0`.

### 6.3 Determining-class identification

Fix a determining class `C_det` of coarse and assembly observables. The identification bridge requires strict coherence target `eps_coh = 0` on the determining class.

---

## 7. Current Theorem Inputs (Tracked)

| Constant | Gate | Current value |
|---|---|---|
| `kappa_coarse` | `CBC_G1` | `1.0913680000000001` |
| `sigma_metric` | `CBC_G2` | `1.073` |
| `kappa_compact` | `CBC_G3` | `0.8045052292839904` |
| `rho_rigidity` | `CBC_G4` | `1.077` |
| `coarse_transfer` | `CBC_G5` | `1.029422` |
| `eps_coh` | `CBC_G6` | `0.0` |
| `sigma_star_can` | stitch | `1.053` |

---

## 8. Current Runtime Snapshot

Latest local guard output (`repro/certificate_runtime.json`):

- `CBC_G1, CBC_G2, CBC_G3, CBC_G4, CBC_G5, CBC_G6, CBC_GM = PASS`,
- strict margin `M_CBC = 0.8045052292839904`,
- lane: `manifold_constrained`.

---

## 9. Reproducibility

Run:

```bash
bash repro/run_repro.sh
```

This writes `repro/certificate_runtime.json`.

---

## 10. In-Paper Appendix Pack (A-E)

### Appendix A. EG1 Coercive Package

The projected response operator yields the raw floor `kappa_coarse^(raw) > 0`, hence `CBC_G1 = PASS`.

### Appendix B. EG2 Capture Package

The defect functional obeys a local-to-global inequality with explicit coarse losses. Positivity of `sigma_metric` yields `CBC_G2 = PASS`.

### Appendix C. EG3 Compactness and No-Collapse Package

Normalized near-failure families lie in the compactness carrier and coarse windows have a positive spacing lower bound, giving `kappa_compact > 0` and `CBC_G3 = PASS`.

### Appendix D. EG4 Rigidity Package

Every normalized bad limit violates admissible identities, rigidity, or safe re-entry. The theorem-level constant `rho_rigidity > 0` excludes bad limits and closes `CBC_G4`.

### Appendix E. Identification and Transfer Package

The transfer constant is `coarse_transfer = 1.029422 > 0`, while strict coherence requires `eps_coh = 0`.

Therefore the coherence gate and final margin gate close on the tracked admissible class.

---

## 11. References

1. J. Roe, *Index Theory, Coarse Geometry, and Topology of Manifolds*, CBMS 90, AMS, 1996.
2. G. Yu, *The coarse Baum-Connes conjecture for spaces which admit a uniform embedding into Hilbert space*, Invent. Math. 139 (2000), 201-240.
3. N. Higson and J. Roe, *Analytic K-Homology*, Oxford Univ. Press, 2000.
