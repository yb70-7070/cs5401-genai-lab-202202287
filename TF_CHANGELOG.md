# TensorFlow version drift log — evidence for A1

Recorded: 2026-10-08T12:50:13.116661 UTC

The course docker-compose.yml pins an older Python/TensorFlow/Keras stack.
Google Colab provides a much newer stack. This file records every drift
and the mitigation applied.

## Drift #0 — Keras backend forced to legacy

- Course target: Keras 2 (tf.keras APIs as written in the notebooks).
- Colab default: TF 2.21.0 would default to Keras 3.
- Mitigation: os.environ["TF_USE_LEGACY_KERAS"] = "1" set before import.
- Verification: tf_keras.__version__ reports 2.21.0.
- Effect: notebooks run unmodified so far.

## Drift #1 — Colab now runs Python 3.13

- Course pin: Python ~3.10/3.11.
- Colab now: 3.13.16.
- Impact so far: none. No distutils-dependent code in the notebooks.

## Drift #2 — TensorFlow now 2.21.0

- Course pin: TF ~2.15.x.
- Colab now: 2.21.0.
- Impact so far: none observed. Further entries appended as needed.
