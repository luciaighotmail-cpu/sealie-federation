# Sealie Federation

**Canonical entry point for the Sealie Federation substrate.**

## Gate Status (2026-10-11)

| Gate | Status |
|------|--------|
| L-01 Repository Authority | **SUPPORTED** — Public repositories verified |
| L-02 Runtime Integration | **SUPPORTED** — Command contract, state machine, authority registry, nonce, interlock implemented in LegionCore |
| L-03 Authority Verification (unit-level) | **SUPPORTED** — internal unit-level evidence |
| L-04 Canonicalization | NOT YET PASSED |
| L-05 Cryptographic Authority | NOT YET PASSED |
| L-06 Merkle Evidence | **SUPPORTED** — full tree + inclusion proofs over current L-03 artefacts |
| L-07 Replay Protection | NOT YET PASSED (harness coverage exists; gate not claimed) |
| Public-market readiness | NOT YET PROVEN |

**Invariant:** No green status without machine-generated evidence. Narrative claims are not evidence.

### L-03 Evidence Reference

| Field | Value |
|-------|-------|
| Evidence ID | `L03-EVIDENCE-20261011T073749Z` |
| Content digest (SHA-256) | `ce7cfc0931b5d6ac228755a502421ca8519e2b061c61827da55eed698a8e36c1` |
| Evidence commit (legioncore) | `c0ff444c8ca5176fb046c5290d302b5a4121cf64` |
| Claim | SUPPORTED (internal unit-level only — not PROVEN) |

### L-06 Merkle Tree Reference

| Field | Value |
|-------|-------|
| Tree ID | `L06-MERKLE-TREE-20261011` |
| Root (SHA-256) | `88f7474c419c03fd63dbf9b9fdd64a3db549c45d9cf0730e140082ff0397c022` |
| Leaves | 4 |
| Depth | 2 |
| Inclusion proofs | All verified at construction |
| Claim | SUPPORTED (tree + proofs exist — not PROVEN) |

Independent verification of L-03 performed 2026-10-11. Merkle tree constructed and proofs verified the same day.

## Sovereign Authority Model

```
                 RAHMAEL
          Sovereign Authority Identity
                     │
              Governance Layer
                     │
              Authority Registry
                     │
             ┌───────┴───────┐
             │               │
        Key Identity      Role Policy
             │               │
       Ed25519 Key ID    SealieGovernor
             │               │
             └───────┬───────┘
                     │
              Authority Token
                     │
                LegionCore
                     │
             Command Interlock
```

- **RAHMAEL-ROOT-001** = governance identity (not a private key)
- Private keys **never** enter GitHub
- GitHub holds: public keys, Key IDs, policy digests, fingerprints, revocation state, evidence references

## Core Repositories

| Repository | Purpose |
|------------|---------|
| [luci](https://github.com/luciaighotmail-cpu/luci) | LUCI / LUCI OMNIS cognitive OS |
| [luci-prime](https://github.com/luciaighotmail-cpu/luci-prime) | Luci Prime Control Desk (Tower / Luci / Nodes / Ledger / Vault / Orders) — MODEL |
| [legioncore](https://github.com/luciaighotmail-cpu/legioncore) | LegionCore distributed substrate |
| [sealie-digital-twin](https://github.com/luciaighotmail-cpu/sealie-digital-twin) | Digital Twin R01 (OMNIS) — synthetic service + observer — MODEL |
| [sealie-os](https://github.com/luciaighotmail-cpu/sealie-os) | Sealie.OS for Lumina nodes |
| [lvx-900](https://github.com/luciaighotmail-cpu/lvx-900) | LVX-900 symbiotic terminal |
| [evidence-ledger](https://github.com/luciaighotmail-cpu/evidence-ledger) | Merkle evidence system |
| [venom-telemetry](https://github.com/luciaighotmail-cpu/venom-telemetry) | Project Venom data pipeline |
| [venom-ai](https://github.com/luciaighotmail-cpu/venom-ai) | Venom ML model suite |
| [omnis](https://github.com/luciaighotmail-cpu/omnis) | Project OMNIS energy+compute |
| [sealie-architecture](https://github.com/luciaighotmail-cpu/sealie-architecture) | L-01–L-07 specifications |
| [sealie-governance](https://github.com/luciaighotmail-cpu/sealie-governance) | Governance & corporate evidence |

## Evidence Planes

```
TECHNICAL PROOF  ≠  FINANCIAL PROOF  ≠  LEGAL PROOF
         ↓                 ↓                 ↓
              GOVERNANCE → AUTHORITY → PUBLIC CLAIM
```

---

*Sealie Federation — Institutional readiness programme.*
