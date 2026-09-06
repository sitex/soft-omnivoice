<!-- GSD:project-start source:PROJECT.md -->

## Project

**soft-omnivoice**

`soft-omnivoice` is the personal `sitex` fork of OmniVoice for local multilingual zero-shot TTS, voice cloning, and voice-design experiments. It preserves upstream package, CLI, training, evaluation, and demo surfaces while separating local verification from advertised capabilities.

**Core Value:** The operator can reproduce dependency, import, CLI, and audio-postprocessing checks without downloading or loading pretrained models.

### Constraints

- **Runtime**: Python, PyTorch, TorchAudio, Transformers, and audio tooling — model-backed import paths can be heavyweight.
- **Assets**: pretrained checkpoints are external and locally untracked — onboarding must not stage them.
- **Hardware**: practical inference is GPU-oriented — CPU and RTF expectations remain unverified.
- **Verification**: no `scripts/verify` exists — Phase 1 must create a deterministic model-free gate.

<!-- GSD:project-end -->

<!-- GSD:stack-start source:codebase/STACK.md -->

## Technology Stack

- Python package managed with `pyproject.toml` and `uv.lock`.
- PyTorch/TorchAudio runtime; GPU-first inference with CUDA or Apple MPS documented.
- CLI entry points include demo, inference, batch inference, and training.
- Audio output is 24 kHz in documented examples.

<!-- GSD:stack-end -->

<!-- GSD:conventions-start source:CONVENTIONS.md -->

## Conventions

Conventions not yet established. Will populate as patterns emerge during development.
<!-- GSD:conventions-end -->

<!-- GSD:architecture-start source:ARCHITECTURE.md -->

## Architecture

# Architecture

The Python package exposes `OmniVoice` model loading and generation. Model, data, training, evaluation, utility, and CLI concerns are separated under `omnivoice/`. Generation supports auto voice, voice cloning, and voice design, with audio post-processing including the already-saved pad/fade behavior.
<!-- GSD:architecture-end -->

<!-- GSD:skills-start source:skills/ -->

## Project Skills

No project skills found. Add skills to any of: `.claude/skills/`, `.agents/skills/`, `.cursor/skills/`, `.github/skills/`, or `.codex/skills/` with a `SKILL.md` index file.
<!-- GSD:skills-end -->

<!-- GSD:workflow-start source:GSD defaults -->

## GSD Workflow Enforcement

Before using Edit, Write, or other file-changing tools, start work through a GSD command so planning artifacts and execution context stay in sync.

Use these entry points:

- `$gsd-quick` for small fixes, doc updates, and ad-hoc tasks
- `$gsd-debug` for investigation and bug fixing
- `$gsd-execute-phase` for planned phase work

Do not make direct repo edits outside a GSD workflow unless the user explicitly asks to bypass it.
<!-- GSD:workflow-end -->

<!-- GSD:profile-start -->

## Developer Profile

> Profile not yet configured. Run `$gsd-profile-user` to generate your developer profile.
> This section is managed by `generate-claude-profile` -- do not edit manually.
<!-- GSD:profile-end -->
