# Federation Control Tower — Master Register

**Date:** 2026-10-20 SAST  
**Invariant:** AUTHORITY ≤ VERIFIED PROOF

## Active packages

| ID | Repo | Status | Notes |
|----|------|--------|-------|
| LP-001 | [luci-prime](https://github.com/luciaighotmail-cpu/luci-prime) | MODEL | Control Desk core modules + public assets on main |
| DT-R01 | [sealie-digital-twin](https://github.com/luciaighotmail-cpu/sealie-digital-twin) | MODEL | Service + 12 tests + observer + docs; release notes for `v0.1.0-r01` |
| LC | [legioncore](https://github.com/luciaighotmail-cpu/legioncore) | SUPPORTED (L-02/L-03 unit) | C++ substrate; internal L-03/L-06 evidence only |
| SF | [sealie-federation](https://github.com/luciaighotmail-cpu/sealie-federation) | SUPPORTED | Canonical entry; repo table updated |
| OMNIS | [omnis](https://github.com/luciaighotmail-cpu/omnis) | MODEL docs | Linked to digital-twin |
| LUCI | [luci](https://github.com/luciaighotmail-cpu/luci) | UNVERIFIED impl | README links Control Desk |

## Release tags (human create — connector has no create-release)

| Tag | Repo | Notes file |
|-----|------|------------|
| `v0.1.0-r01` | sealie-digital-twin | `RELEASE_NOTES_v0.1.0-r01.md` |
| `v0.1.0` | luci-prime | `RELEASE_NOTES_v0.1.0.md` |

## Blockers

- No create_tag / create_release in GitHub connector
- Full interactive Luci Prime UI body primarily in session working tree (core contracts on GitHub)
- Unreal / Pixel Streaming / measured data: UNVERIFIED

## Gates requiring explicit approval

1. Human publishes release tags from notes files
2. Full `src/app.ts` interactive module commit to luci-prime
3. Digital Twin R02 scope
4. Any production deploy or spend
