# Integrations

- Upstream/vendor lineage: k2-fsa/OmniVoice.
- Pretrained model source is Hugging Face; local `pretrained_models/` is user-owned and untouched.
- Optional evaluation/training integrations use datasets, Accelerate, and GPU toolchains.
- CLI surfaces are implemented under `omnivoice/cli/`.

No model download or heavy inference was performed during onboarding.
