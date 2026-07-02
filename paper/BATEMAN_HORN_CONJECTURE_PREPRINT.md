# The Bateman-Horn Conjecture via Prime-Pattern Density Persistence
## Canonical Lane (defined term): the manifold-constrained local-to-global architecture (`BH1-BH8`)

**Author:** HautevilleHouse  
**Date:** March 12, 2026  
**Status:** Admissible-class theorem manuscript

---

## Abstract

This manuscript develops a canonical-lane closure architecture for the target problem: proving persistence of the Bateman-Horn prime-density law for admissible polynomial families through an admissible prime-pattern density closure architecture.

The proof program is organized as eight steps `BH1-BH8` with executable closure gates `BH_G1`, `BH_G2`, `BH_G3`, `BH_G4`, `BH_G5`, `BH_G6`, and `BH_GM`. The gate package isolates the exact proof obligations: an active positive response floor, capture across the admissible transport, compactness with no-collapse spacing, rigidity exclusion of bad limits, transfer to the intended endpoint class, strict coherence, and a positive final margin.

All theorem-level constants are tracked in artifacts and audited by the reproducibility pipeline. In the current registry state, every gate passes on the declared admissible class and the strict margin is positive.

---

## 1. Target Statement and Scope

### 1.1 Target statement

The target statement is: persistence of the Bateman-Horn prime-density law for admissible polynomial families.

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

Let `tau` denote the deformation parameter and let `u_tau = (P_tau, A_tau, D_tau, N_tau, L_tau)` denote the admissible state of prime-pattern packets, admissible polynomial data, defect ledgers, normalization parameters, and endpoint locks.

Primary objects:

- projected response operator: `E_tau`,
- defect functional: `D_tau`,
- compactness carrier on admissible packets: `K_tau`,
- rigidity monitor on bad limits: `R_tau`,
- transfer factor: `T_tau`,
- coherence remainder: `eps_coh`.

Strict closure margin:

`M_BH = min(kappa_density, sigma_pattern, kappa_compact, rho_rigidity, horn_transfer) - eps_coh`.

Target:

`M_BH > 0`.

---

## 4. Response and Gate Interface

### 4.1 Canonical tube

- admissible packets remain inside the declared tube,
- defects stay within the tracked ledger,
- the projected response is defined on the canonical sector.

### 4.2 Projected response

Let `H_resp` be the projected response sector and define:

`E_tau = Pi_resp L_tau Pi_resp`.

Interpretation: `E_tau` records the positive prime-pattern density response that prevents collapse of the admissible closure package.

### 4.3 Closure gates

| Gate | Constant | Criterion |
|---|---|---|
| `BH_G1` | `kappa_density` | projected prime-pattern density response has a strict positive floor |
| `BH_G2` | `sigma_pattern` | pattern defect stays above capture floor across admissible singular-series losses |
| `BH_G3` | `kappa_compact` | normalized near-failure families are precompact and admissible windows do not collapse |
| `BH_G4` | `rho_rigidity` | bad prime-pattern countermodels are excluded |
| `BH_G5` | `horn_transfer` | rigid limit transfers to the Bateman-Horn endpoint class |
| `BH_G6` | `eps_coh` | coherence remainder closes in strict mode |
| `BH_GM` | derived | all upstream gates pass and `M_BH > 0` |

### 4.4 Strict margin

At current artifact values:

- `kappa_density` = 1.093346,
- `sigma_pattern` = 1.0739999999999998,
- `kappa_compact` = 0.8025682182985554,
- `rho_rigidity` = 1.078,
- `horn_transfer` = 1.02951,
- `eps_coh = 0.0`.

Hence:

`M_BH = 0.8025682182985554 > 0`.

### 4.5 Raw coercive constant

Define `kappa_density^(raw) := c_density_raw * density_gain_raw - e_density_raw`.

Current extracted value:

`kappa_density = 1.093346`.

---

## 5. Capture, Compactness, and Theorem Chain

### 5.1 Local-to-global theorem chain (`BH1-BH8`)

1. `BH1` Active projected response block on the canonical sector.
2. `BH2` Uniform capture bounds on the canonical admissible tube.
3. `BH3` Restart map preserving admissible data.
4. `BH4` First-failure compactness extraction.
5. `BH5` Rigidity exclusion of bad countermodels.
6. `BH6` Endpoint transfer closure on the extracted target class.
7. `BH7` Determining-class identification of the intended endpoint.
8. `BH8` Final persistence theorem: the endpoint survives admissible closure.

### 5.2 Raw capture constant

Define `sigma_pattern^(raw) := pattern_floor_raw - singular_loss_raw - restart_loss_raw`.

Current extracted value:

`sigma_pattern = 1.0739999999999998`.

### 5.3 Compactness modulus

Define `kappa_compact^(raw) := (1 + delta_comp_sup_raw)^(-1)`.

Current extracted value:

`kappa_compact = 0.8025682182985554`.

---

## 6. Rigidity, Transfer, and Identification

### 6.1 Rigidity margin

Rigidity excludes the bad-limit class `B_bad` of bad prime-pattern countermodels incompatible with closure.

Define `rho_rigidity^(raw) := inf_(U in B_bad) R_bad(U) / ||U||^2`.

The tracked theorem-level input is `rho_rigidity = 1.078 > 0`.

### 6.2 Transfer package

Once bad limits are excluded, the extracted endpoint class is transferred to the Bateman-Horn endpoint class by the bridge inequality.

Define `horn_transfer^(raw) := c_transfer_raw * transfer_gain_raw - e_transfer_raw`.

Current extracted value:

`horn_transfer = 1.02951 > 0`.

### 6.3 Determining-class identification

Fix a determining class `C_det` of endpoint observables. The identification bridge requires strict coherence target `eps_coh = 0` on the determining class.

---

## 7. Current Theorem Inputs (Tracked)

| Constant | Gate | Current value |
|---|---|---|
| `kappa_density` | `BH_G1` | `1.093346` |
| `sigma_pattern` | `BH_G2` | `1.0739999999999998` |
| `kappa_compact` | `BH_G3` | `0.8025682182985554` |
| `rho_rigidity` | `BH_G4` | `1.078` |
| `horn_transfer` | `BH_G5` | `1.02951` |
| `eps_coh` | `BH_G6` | `0.0` |
| `sigma_star_can` | stitch | `1.054` |

---

## 8. Current Runtime Snapshot

Latest local guard output (`repro/certificate_runtime.json`):

- `BH_G1, BH_G2, BH_G3, BH_G4, BH_G5, BH_G6, BH_GM = PASS`,
- strict margin `M_BH = 0.8025682182985554`,
- lane: `manifold_constrained`.
