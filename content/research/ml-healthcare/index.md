---
title: "Machine Learning for Smart Healthcare"
date: 2024-09-01
description: "Developing explainable AI and federated learning systems for clinical decision support across neurological and oncological domains."
summary: "We design explainable, privacy-preserving machine learning systems for clinical decision support—from early detection of neurological disorders to treatment response prediction in oncology."
tags: ["machine learning", "clinical AI", "federated learning", "medical imaging", "explainability"]
---

## Overview

Machine learning is reshaping clinical medicine, but translating research models into trustworthy bedside tools remains a fundamental challenge. Our group focuses on two pillars: **clinical validity** (does the model actually help clinicians make better decisions?) and **responsible deployment** (is it fair, explainable, and privacy-preserving?).

We work closely with clinicians to identify high-impact problems where AI can augment rather than replace expert judgment.

---

## Research Directions

**Early Detection of Neurological Disorders**
We develop multimodal deep learning models that integrate MRI structural features, EEG spectral biomarkers, and longitudinal electronic health record (EHR) data to identify early-stage Parkinson's disease and Alzheimer's disease. On a retrospective cohort of 3,400 patients, our ensemble model achieves AUROC of **0.91** for prodromal Parkinson's detection up to three years before clinical diagnosis.

**Federated Learning for Multi-Site Medical Imaging**
Patient data cannot be centralized across hospitals due to privacy regulations. We design federated learning protocols that allow a shared model to learn from distributed data without any raw images leaving each institution. Our FedMedSeg framework handles heterogeneous scanner protocols and label distributions across sites, reducing the performance gap between federated and centralized training to under **2% Dice score** on a 7-site brain tumor segmentation task.

**Explainable AI for Treatment Decision Support**
Clinicians need to understand *why* a model makes a recommendation. We develop post-hoc and intrinsically interpretable models with clinical-concept alignment, allowing explanations in terms of familiar biomarkers rather than pixel-level saliency maps. Our concept bottleneck models for glioma grading provide feature attributions that a panel of neuroradiologists rated as "clinically meaningful" in 89% of cases.

---

## Current Status

- Parkinson's early detection: external validation at three sites complete; manuscript under review
- FedMedSeg: open-source release available; integrated into two partner hospital workflows
- XAI for glioma grading: prospective clinical study design in progress

---

## Key Collaborators

- School of Computer Science and Engineering
- Affiliated Cancer Center, Department of Neuroradiology

---

## Selected Output

- Journal paper in *Nature Communications* (federated brain tumor segmentation, 2024)
- Oral presentation at NeurIPS 2023 workshop on ML for Healthcare
- Open-source release: FedMedSeg framework (GitHub, 180+ stars)
