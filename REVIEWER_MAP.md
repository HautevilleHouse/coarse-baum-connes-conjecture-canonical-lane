# Reviewer Map

    ## Claim Scope

    - Canonical-lane claim: inside the `manifold_constrained` lane, if the theorem chain in this repository holds and the guard certificate passes, the repository-level closure claim is satisfied.
    - Standard target claim: carried by the in-repo bridge theorems tying the lane to the target statement.

    ## Theorem Dependency Chain

    1. `EG1`: coercive response and active control floor.
    2. `EG2`: capture and admissible continuation.
    3. `EG3`: compactness and no-collapse spacing.
    4. `EG4`: rigidity and transfer.
    5. Identification bridge: strict coherence on the determining class.
    6. Scalar closure: `CBC_G1, CBC_G2, CBC_G3, CBC_G4, CBC_G5, CBC_G6, CBC_GM` all `PASS`.

    Primary files:

    - `paper/COARSE_BAUM_CONNES_CONJECTURE_PREPRINT.md`
    - `notes/EG1_public.md`
    - `notes/EG2_public.md`
    - `notes/EG3_public.md`
    - `notes/EG4_public.md`
    - `notes/IDENTIFICATION_BRIDGE.md`

    ## Closure Gates

    | Gate | Constant | Description |
    |------|----------|-------------|
    | `CBC_G1` | `kappa_coarse` | projected coarse response has a strict positive floor |
| `CBC_G2` | `sigma_metric` | metric defect stays above capture floor across admissible coarse losses |
| `CBC_G3` | `kappa_compact` | normalized near-failure families are precompact and coarse windows do not collapse |
| `CBC_G4` | `rho_rigidity` | bad nonisomorphic coarse countermodels are excluded |
| `CBC_G5` | `coarse_transfer` | rigid limit transfers to the coarse-assembly endpoint class |
| `CBC_G6` | `eps_coh` | strict coherence / identification closure |
| `CBC_GM` | derived | final strict margin |

    ## Falsification Conditions

    - `repro/certificate_runtime.json` has any non-`PASS` gate.
    - `lane.active_lane != "manifold_constrained"`.
    - `all_pass != true`.
    - Any manifest hash mismatch under `repro/repro_manifest.json`.
    - A verified counterexample to any EG theorem statement used in the paper.
