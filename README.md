# Sealie Federation

**Canonical entry point for the Sealie Federation substrate.**

## Gate Status (2026-08-22)

| Gate | Status |
|------|--------|
| L-01 Repository Authority | **UNBLOCKED** — Public repositories verified |
| L-02 Runtime Integration | **NEXT** — Interfaces & command contract in progress |
| L-03 Authority Verification | NOT YET PASSED |
| L-04 Canonicalization | NOT YET PASSED |
| L-05 Cryptographic Authority | NOT YET PASSED |
| L-06 Merkle Evidence | NOT YET PASSED |
| L-07 Replay Protection | NOT YET PASSED |
| Public-market readiness | NOT YET PROVEN |

**Invariant:** No green status without machine-generated evidence. Narrative claims are not evidence.

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
| [legioncore](https://github.com/luciaighotmail-cpu/legioncore) | LegionCore distributed substrate |
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
