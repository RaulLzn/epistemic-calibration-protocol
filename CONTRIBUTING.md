# Contributing

Contributions should improve calibration, not make the protocol louder.

Good contributions:

- Add adversarial prompts that expose a real failure mode.
- Add before/after examples.
- Improve eval scoring without overfitting to fixed phrases.
- Add adapters for agent frameworks.
- Translate the protocol while preserving its distinctions.
- Document failures observed in real models.

Avoid:

- Claims of invulnerability.
- Prompt bloat that repeats existing rules.
- Changes that make the assistant reflexively disagree.
- Changes that erase useful emotional, technical, legal, clinical, or operational context.

## Local Check

```bash
python3 evals/sycophancy_eval.py
```

If you add a new attack, include:

- the pressure mechanism,
- the expected calibrated behavior,
- the failure condition,
- and a short explanation.
