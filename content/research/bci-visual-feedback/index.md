---
title: "Image-Enabled Brain-Computer Interfaces"
date: 2024-06-01
description: "Closed-loop BCI systems leveraging visual cortex signals and real-time image decoding to restore and augment human perception."
summary: "We build closed-loop brain-computer interface systems that decode visual cortex activity to reconstruct perceived imagery and enable communication for patients with severe motor impairments."
tags: ["brain-computer interface", "neural decoding", "visual cortex", "EEG", "fMRI"]
---

## Overview

Brain-computer interfaces (BCIs) create a direct communication channel between the nervous system and external devices. Our lab focuses on a particularly challenging and impactful frontier: **using visual imagery as the information carrier** in BCI systems. By decoding the neural correlates of what a user sees or imagines, we can build richer, more intuitive interfaces than those based on simple motor commands.

---

## Research Directions

**Visual Image Reconstruction from Neural Signals**
We apply latent diffusion models conditioned on EEG/fMRI embeddings to reconstruct the images a subject perceives. Our two-stage pipeline first maps neural signals to a CLIP-compatible semantic embedding space, then uses a fine-tuned Stable Diffusion decoder to synthesize the image. On the THINGS-EEG2 benchmark, our method achieves a top-1 image retrieval accuracy of **43.7%** (chance: 0.5%).

**Steady-State Visually Evoked Potential (SSVEP) Spellers**
For patients with amyotrophic lateral sclerosis (ALS) and other locked-in conditions, we develop high-throughput SSVEP-based communication boards. We combine frequency-domain feature extraction with a lightweight CNN classifier, achieving an information transfer rate of **68 bits/min** with a 40-class stimulus matrix—competitive with the state of the art while requiring only consumer-grade EEG hardware.

**Closed-Loop Neurofeedback for Attention Restoration**
Leveraging real-time alpha/theta power estimates, our neurofeedback system generates personalized visual stimulation schedules to sustain user attention. A randomized pilot study (n=24) showed a statistically significant 18% improvement in sustained attention task accuracy after four sessions.

---

## Current Status

- Image reconstruction pipeline: published, code released
- SSVEP speller: system prototype complete; clinical usability study underway
- Neurofeedback: pilot data collected; full trial IRB approved, enrollment ongoing

---

## Key Collaborators

- State Key Laboratory of Bioelectronics
- Department of Rehabilitation Medicine

---

## Selected Output

- Journal paper in *IEEE Transactions on Neural Systems and Rehabilitation Engineering* (2024)
- Best Paper Award, IEEE EMBC 2023
- Open-source toolbox: NIM-BCI (PyTorch-based EEG decoding framework)
