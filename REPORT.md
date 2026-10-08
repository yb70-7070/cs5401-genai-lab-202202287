# CS5401 Generative AI Lab — REPORT

**Author:** yb70-7070
**Repository:** https://github.com/yb70-7070/cs5401-genai-lab-202202287
**Date:** 2026-10-08

## Reproduction commands

Run these in Google Colab (Docker was not runnable on the host machine).

    import os
    os.environ["TF_USE_LEGACY_KERAS"] = "1"   # before importing tensorflow
    !git clone https://github.com/khobatha/CS5401.git /content/CS5401

Then open the notebook in `lab-genai/` and Run All.

## A1 — Environment

| Item | Value |
|---|---|
| Baseline commit (course repo) | `208a175112ebd8ff02761d179a6032005850f6f9` |
| Platform | Google Colab (free tier) — Docker unavailable on host |
| Python | 3.13.16 |
| TensorFlow | 2.21.0 |
| Keras backend | tf_keras 2.21.0 (legacy Keras 2) |
| OS | Linux-6.6.122+-x86_64-with-glibc2.39 |
| CPU | x86_64 |
| CPU cores | 2 |
| RAM (GB) | 13.6 |
| GPU | none |
| Build time | N/A — no Docker build; Colab prebuilt image |
| Download volume | TBD — fill after first CIFAR-10 download |

### Version drift

Colab ships much newer Python and TensorFlow than the course's Dockerfile pins.
`TF_USE_LEGACY_KERAS=1` restores the Keras 2 API the notebooks expect.
Every drift-driven change is logged in `TF_CHANGELOG.md`.

## A2 — Baseline numbers

(to be filled after Part B)

## A3 — Cost of the lab

(to be filled)
