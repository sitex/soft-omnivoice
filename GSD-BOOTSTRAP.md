---
document: gsd-brownfield-bootstrap
project: soft-omnivoice
git_root: /home/rocky/projects/soft-omnivoice
github_repository: sitex/soft-omnivoice
generated_at: 2026-09-06T02:03:45Z
thoughts_status: canonical shared baseline available
github_status: repository resolved; Issues API unavailable or disabled for this fork
include_personal: false
---

# Purpose

Vendor clone of OmniVoice for multilingual zero-shot TTS, voice cloning, and voice design. [T1]

# Implemented Capabilities

- Python package and CLI surfaces for demo, inference, batch inference, and training. [T1]
- Documented 600+ language support, cloning, design, auto voice, controls, and generation parameters. [T1]
- `uv` lock metadata is present; pad/fade behavior is saved in history. [T1]

# Current Milestone

Active v1: local reproducible build/smoke baseline and hardware/model constraint capture. [T1]

# Open Requirements

- Verify dependency/import and CLI-help smoke checks without loading pretrained models. [T1]
- Verify model-backed multilingual generation, cloning quality, and RTF when assets/hardware permit. [T1]

# Accepted Decisions

- Preserve existing pad/fade behavior and lockfile normalization commits. [T1]
- Leave untracked `pretrained_models/`, `src/`, and `tests/` untouched. [T1]
- Do not download models or run heavy inference during onboarding. [T1]

# Constraints

- PyTorch/TorchAudio and pretrained checkpoints are required for real generation. [T1]
- Fast inference is GPU-oriented; CPU and claimed RTF remain unverified. [T1]

# Unresolved Conflicts

None identified from available sources.

# Source Thoughts

- [T1 baseline](/home/rocky/thoughts/repos/soft-omnivoice/shared/research/2026-09-06-project-baseline.md)
- [T1 plan](/home/rocky/thoughts/repos/soft-omnivoice/shared/plans/2026-09-06-gsd-onboarding.md)

# Source Issues

None included; the Issues API is unavailable or disabled for this fork.

# Source Limitations

Claims are source- and repository-inspection-based, not model-backed verification.
