# Reduplicated Adjectives · Sentiment Shift

Undergraduate thesis research (supervised by **Lecturer Dezhi Cao**): whether Chinese adjective reduplication (AABB / ABB) shifts contextual sentiment polarity relative to base forms in informal social-media language.

## Pipeline

**Corpus construction → LLM scoring → human gold validation → statistical testing**

1. Harvested and cleaned Weibo text into **14,987** valid sentence instances covering **22** base–reduplicated adjective pairs (11 AABB + 11 ABB; raw harvest 22,531 → cleaned set).
2. Scored contextual polarity with **DeepSeek-V3** on a 1–5 Likert scale via iterative structured prompts.
3. Benchmarked model scores against a three-annotator majority-vote gold standard on **1,486** stratified samples → **Exact Match 97.11%**.
4. Compared base vs reduplicated scores with a two-sample **Welch's *t*-test**.

## Locked results

| Contrast | What it compares | Result |
|----------|------------------|--------|
| **Overall Welch** | Base vs reduplicated sentence scores (**n = 14,987**) | *t* = 2.49, **p = 0.013**, aggregate Δ ≈ −0.04, \|*d*\| ≈ 0.04 |
| Pair-level Δ | 22 adjective pairs | Δ ∈ [−0.66, +0.74] (heterogeneous direction/magnitude) |
| **AABB group** | Pair-level mean Δ within AABB (**n = 11**) | mean Δ ≈ +0.10, **p ≈ 0.193** |
| **ABB group** | Pair-level mean Δ within ABB (**n = 11**) | mean Δ ≈ −0.04, p ≈ 0.744 |

**Interpretation note:** **p = 0.013** is the overall base–reduplicated Welch test. **p ≈ 0.193** is the AABB *group-level* mean-Δ test — a different contrast, not a second report of the overall effect.

## Key figures

<p align="center">
  <img src="./fig09_delta_heterogeneity.png" alt="Fig.9 pair-level Δ heterogeneity" width="48%" />
  <img src="./fig10_aabb_abb_group_comparison.png" alt="Fig.10 AABB vs ABB group comparison" width="48%" />
</p>

- **Fig.9** — Pair-level sentiment polarity shift (Δ) across 22 reduplicated adjective pairs (heterogeneity / continuous distribution).
- **Fig.10** — AABB vs ABB group comparison of pair-level mean Δ (AABB p≈0.193 ≠ overall Welch p=0.013).

Figures are thesis artefacts (synced with the final draft charts), not a separate web demo.

## Profile

Portfolio summary: [github.com/yuanyiqi422-byte](https://github.com/yuanyiqi422-byte)
