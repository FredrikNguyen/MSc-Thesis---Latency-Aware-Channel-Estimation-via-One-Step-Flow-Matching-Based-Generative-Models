# Flow Matching for Efficient Channel Estimation in MIMO-OFDM 
Master's thesis: Channel-Estimation-via-One-Step-Flow-Matching-Based-Generative-Models. PyTorch implementation of flow matching generative models for efficient channel estimation in pilot-contaminated MIMO-OFDM. 

**Status:** Finished Master's Thesis Project (KTH x Huawei Sweden R&D, 2026)

## Motivation
Accurate and low-latency channel estimation is a core requirement in modern wireless receivers. In difficult operating conditions such as low SNR and pilot contamination, classical estimators can become limited. This project explores whether recent generative modeling ideas, especially flow matching and related one-step objectives, can be adapted to produce better channel estimates while still remaining practical for latency-constrained wireless systems.

# Abstract

Accurate channel state information is essential for reliable wideband massive MIMO-OFDM systems, but pilot contamination and noise make channel estimation difficult, while practical deployment also favors estimators with low inference cost. This thesis studies whether conditional flow-matching-based one-step estimators can improve channel estimation under pilot contamination in wideband massive MIMO-OFDM systems.

The task is formulated as supervised recovery of the desired channel from projected noisy least-squares pilot observations. The observations are processed in the delay-beam domain, and the learned estimators are compared with a hard-windowing baseline and an ideal upper bound. The study evaluates one-step variants of standard flow matching, Mean Flow, data-parameterized flow, and consistency-style endpoint models, together with ablations over source-state choice, context conditioning, backbone architecture, training signal-to-noise-ratio distribution, and teacher-student distillation. Evaluation combines offline reconstruction diagnostics with end-to-end symbol error rate in a simulator.

The results show that the strongest reported one-step flow-based models yield modest gains over hard-windowing when the model design is aligned more closely with the channel-estimation task. Mean Flow improves over naive one-step standard flow, while the strongest reported one-step result is achieved by combining observation-anchored denoising, consistency-style endpoint learning, focused low-signal-to-noise-ratio training, and teacher-student distillation. This distilled one-step student, compressed from a roughly 4 million parameter teacher to roughly 50 thousand parameters, achieves a gain of 0.66 dB at symbol error rate 0.1 over hard-windowing, corresponding to about 14% less required linear signal-to-noise ratio. The thesis therefore shows that learned one-step channel estimation can improve end-to-end communication performance in the studied simulated pilot-contaminated setting.

## Keywords

Channel estimation, Wireless communications, Massive multiple-input multiple-output systems, Orthogonal frequency-division multiplexing, Pilot contamination, Flow matching, Consistency models, Mean Flow models, Distillation, Delay-beam domain, End-to-end communication evaluation, Low-latency inference, One-step inference

## Methodology & Tech Stack
- **Framework:** PyTorch-based modeling workflow
- **Core Methods:** Flow Matching, Consistency-style one-step objectives, and CMT-based distillation
- **Problem Setting:** Pilot-contaminated wideband massive MIMO-OFDM channel estimation
