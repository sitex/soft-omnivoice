# soft-omnivoice

## What This Is

`soft-omnivoice` is the personal `sitex` fork of OmniVoice for local multilingual zero-shot TTS, voice cloning, and voice-design experiments. It preserves upstream package, CLI, training, evaluation, and demo surfaces while separating local verification from advertised capabilities.

## Core Value

The operator can reproduce dependency, import, CLI, and audio-postprocessing checks without downloading or loading pretrained models.

## Requirements

### Validated

- ✓ Python package, demo, inference, batch inference, training, and evaluation surfaces exist — existing repository
- ✓ Voice cloning, voice design, auto voice, and multilingual controls are represented in source and documentation — existing code and docs
- ✓ Local pad/fade behavior and normalized dependency lock metadata are preserved in published commits — portfolio history

### Active

- [ ] Reproduce the locked environment and import the supported package boundary without downloading models.
- [ ] Run model-free CLI help or argument-validation checks for supported entry points.
- [ ] Add a deterministic model-free check for the saved audio pad/fade behavior.

### Out of Scope

- Downloading or committing pretrained weights during onboarding — `pretrained_models/` remains local and untracked.
- Claiming multilingual generation, cloning quality, or RTF without model-backed execution.
- Committing the existing untracked package/test stubs — their intent is unresolved.

## Context

The fork originates from `k2-fsa/OmniVoice`. The local checkout diverged from upstream and is preserved as `origin/portfolio` without rewriting vendor history. Commits `8e86fcd` and `0334598` preserve the local pad/fade change and verified lock normalization. Evidence lives in `GSD-BOOTSTRAP.md`, `.planning/codebase/`, and canonical HumanLayer Thoughts.

## Constraints

- **Runtime**: Python, PyTorch, TorchAudio, Transformers, and audio tooling — model-backed import paths can be heavyweight.
- **Assets**: pretrained checkpoints are external and locally untracked — onboarding must not stage them.
- **Hardware**: practical inference is GPU-oriented — CPU and RTF expectations remain unverified.
- **Verification**: no `scripts/verify` exists — Phase 1 must create a deterministic model-free gate.

## Key Decisions

| Decision | Rationale | Outcome |
|----------|-----------|---------|
| Preserve pad/fade and lock changes as separate commits | Keep functional and mechanical history reviewable | ✓ Good |
| Keep pretrained assets untracked | Avoid publishing large or restricted model files | ✓ Good |
| Verify model-free boundaries before model inference | Establish a bounded reproducible baseline | — Pending |

## Evolution

This document evolves at phase transitions and milestone boundaries.

**After each phase transition**:
1. Move verified model-free requirements to Validated with evidence.
2. Record asset and hardware blockers without converting them into passes.
3. Update constraints and decisions discovered during execution.
4. Recheck the maintained-fork description and core value.

**After each milestone**:
1. Review requirement and asset status.
2. Reconfirm the upstream/fork boundary.
3. Define the next evidence-backed milestone.

---
*Last updated: 2026-09-06 after brownfield initialization*
