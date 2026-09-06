# Roadmap: soft-omnivoice

## Phases

- [ ] **Phase 1: Model-Free Runtime Baseline** - Verify the environment, imports, CLIs, and audio postprocessing without pretrained assets.

## Phase Details

### Phase 1: Model-Free Runtime Baseline
**Goal:** The operator can reproduce the supported model-free package and CLI boundaries and protect the saved pad/fade behavior with deterministic evidence.
**Mode:** mvp
**Depends on:** Nothing (first phase)
**Requirements:** OMNI-01, OMNI-02, OMNI-03
**Success Criteria:**
1. A documented command validates the lock and imports the supported package boundary without downloading or loading models.
2. Supported CLI entry points expose deterministic help or invalid-argument behavior without model assets.
3. A model-free test observes the configured 50 ms pad and 10 ms fade at the audio postprocessing boundary.
4. Hardware and asset limitations are recorded as skips, not passes.
5. A repository verification command runs all model-free checks and reports a nonzero exit on failure.
**Plans:** TBD

## Progress

| Phase | Plans Complete | Status | Completed |
|-------|----------------|--------|-----------|
| 1. Model-Free Runtime Baseline | 0/TBD | Not started | - |
