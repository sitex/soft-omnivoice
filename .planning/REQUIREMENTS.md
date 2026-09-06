# Requirements: soft-omnivoice

**Defined:** 2026-09-06
**Core Value:** Reproduce dependency, import, CLI, and audio-postprocessing checks without pretrained model loading.

## v1 Requirements

### Model-Free Baseline

- [ ] **OMNI-01**: Operator can verify the locked environment and import the supported package boundary without downloading or loading models.
- [ ] **OMNI-02**: Operator can run model-free help or argument-validation checks for the supported CLI entry points and record deterministic exit behavior.
- [ ] **OMNI-03**: Operator can run a deterministic model-free check proving the configured 50 ms pad and 10 ms fade are applied to generated audio postprocessing.

## v2 Requirements

### Model-Backed Runtime

- **OMNI-04**: Operator can generate multilingual speech with approved local assets.
- **OMNI-05**: Operator can verify voice cloning/design quality and record RTF on compatible hardware.

## Out of Scope

| Feature | Reason |
|---------|--------|
| Automatic model downloads | Asset acquisition is operator-controlled. |
| Committing `pretrained_models/` | Large or restricted assets remain local. |
| Existing untracked package/test stubs | Intent and provenance are unresolved. |

## Traceability

| Requirement | Phase | Status |
|-------------|-------|--------|
| OMNI-01 | Phase 1 | Pending |
| OMNI-02 | Phase 1 | Pending |
| OMNI-03 | Phase 1 | Pending |

**Coverage:** 3 total, 3 mapped, 0 unmapped ✓

---
*Requirements defined: 2026-09-06*
*Last updated: 2026-09-06 after brownfield initialization*
