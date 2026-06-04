# Flow Matching for Low-Latency Channel Estimation in MIMO-OFDM
Master's thesis: Latency-Aware-Channel-Estimation-via-One-Step-Flow-Matching-Based-Generative-Models. PyTorch implementation of flow matching generative models for low-latency channel estimation in pilot-contaminated MIMO-OFDM.
**Status:** Master's Thesis Project (KTH x Huawei Sweden R&D, 2026)

## Overview
This repository contains the working material for my Master's thesis on latency-aware channel estimation using one-step generative models for pilot-contaminated wideband MIMO-OFDM systems. The project investigates whether flow-matching-based models can improve end-to-end communication performance under strict inference-cost constraints.

At the moment, this repository is empty but will be updated.  <!--- mainly contains the thesis manuscript, figures, references, experiment summaries, and supporting notes. The code structure is still being organized.-->

## Motivation
Accurate and low-latency channel estimation is a core requirement in modern wireless receivers. In difficult operating conditions such as low SNR and pilot contamination, classical estimators can become limited. This project explores whether recent generative modeling ideas, especially flow matching and related one-step objectives, can be adapted to produce better channel estimates while still remaining practical for latency-constrained wireless systems.
<!---
## Repository Contents
- `thesis_prelim.tex` - main thesis manuscript
- `figures/` - figures and exported thesis visuals
- `sources/` - papers, reports, and reference material used during the study
- `results.txt` - exported simulator and ablation-study summaries
- `references.bib` - bibliography database
- `code/` - placeholder for project code organization
-->
## Methodology & Tech Stack
- **Framework:** PyTorch-based modeling workflow
- **Core Methods:** Flow Matching, Consistency-style one-step objectives, and CMT-based distillation
- **Problem Setting:** Pilot-contaminated wideband massive MIMO-OFDM channel estimation
- **Evaluation:** End-to-end communication metrics in an integrated MIMO-OFDM simulator
- **Writing Stack:** LaTeX using the KTH thesis template

## Current Roadmap
- [x] Literature review on channel estimation, flow matching, consistency, and related generative methods
- [x] Set up classical baselines and simulator evaluation pipeline
- [x] Run ablations over task formulation, context, model family, backbone, and training distribution
- [x] Evaluate consistency and teacher-student CMT distillation for low-latency one-step inference
- [x] Analyze SER, Gain$_{0.1}$, NMSE, latency, and supplementary reconstruction diagnostics
- [ ] Package the repository into a cleaner standalone public code release

## Notes
This repository is still under active development. The thesis manuscript and result summaries are currently the most complete parts of the project, while the code layout is still being cleaned up for easier reuse and publication.
