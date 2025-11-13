# 🤸 Spatio-Temporal Interaction Recognition with ST-GCN

[![Open SBU Notebook](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/GabrielOyetunji/spatio-temporal-interaction-recognition/blob/main/Final__SBU_dataset.ipynb)
[![Open UTI Notebook](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/GabrielOyetunji/spatio-temporal-interaction-recognition/blob/main/Final__UTI_dataset.ipynb)

Skeleton-based Human Interaction Understanding using Enhanced ST-GCN Architectures
...
📌 Spatio-Temporal Interaction Recognition with ST-GCCN & Hybrid Models

Skeleton-based Human Interaction Understanding using Enhanced ST-GCN Architectures

This repository implements and evaluates multiple Spatio-Temporal Graph Convolutional Network (ST-GCN) variants for recognising two-person human interactions using skeleton-sequence data.
The project explores how architectural enhancements — Multi-Stream Fusion, Dilated TCN, SE-Attention, and Transformer-based Temporal Reasoning — affect performance across structured and unstructured datasets.

The work is based on the original ST-GCN (Yan et al., 2018) and extends it with eight experimental variants.

⸻

🚀 Project Overview

Skeleton-based interaction recognition provides a privacy-preserving, noise-robust alternative to RGB-based methods.
However, existing models struggle with:
	•	Changing viewpoints
	•	Occlusions
	•	Non-uniform motion
	•	Unconstrained (real-world-like) recording conditions

This repo evaluates nine distinct architectures across:
	•	SBU Kinect Interaction dataset (structured, clean skeletons)
	•	UT Interaction dataset (unconstrained, noisy, variable sequence lengths)

⸻

🧠 Models Implemented

Baseline
	•	Model 1 – Original ST-GCN (AAAI 2018)

Single-stream Enhancements
	•	Model 2 – Multi-Stream ST-GCN
	•	Model 3 – Dilated-TCN ST-GCN
	•	Model 4 – SE-Attention ST-GCN
	•	Model 5 – Transformer Temporal Head

Multi-stream Hybrids
	•	Model 6 – Multi-Stream + Dilated TCN
	•	Model 7 – Multi-Stream + SE Attention
	•	Model 8 – Multi-Stream + Transformer
	•	Model 9 – Full Hybrid (All Modules Combined)

⸻

📊 Key Results

SBU Kinect Interaction (Structured Dataset)
	•	Full Hybrid (Model 9) achieved the highest performance
	•	Mean Accuracy: 0.981
	•	Mean F1-Score: 0.983
	•	Transformer-enhanced and dilated-TCN models also performed strongly.

UT Interaction (Unconstrained Dataset)
	•	Performance dropped significantly across all models due to noise, occlusion, and viewpoint changes.
	•	Model 8 (Multi-Stream Transformer) achieved the best F1-Score: ~0.459
	•	Shows that temporal reasoning generalises better than pure spatial refinements.