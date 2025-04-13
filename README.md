# 🎯 Emotion Recognition in Conversations – Baseline Models

This repository is part of my PPD Project on **Emotion Recognition in Conversations**. The goal is to benchmark and analyze several state-of-the-art **graph-based and multimodal models** for ERC (Emotion Recognition in Conversation). I selected four well-cited and openly available models as baselines, each representing a different modeling strategy (textual graphs, multimodal GCNs, cross-modal attention, and knowledge distillation).

---

## 📌 Selected Baseline Models

### 🔷 1. DialogueGCN
> I use **DialogueGCN** as a strong **textual baseline**. It models speaker and temporal dependencies via directed conversational graphs and is one of the most cited works in ERC.
- 🔗 **Paper** → [DialogueGCN (Ghosal et al., AAAI 2020)](https://aclanthology.org/2020.aaai-1.590.pdf)
- 💻 **Code** → [declare-lab/conv-emotion](https://github.com/declare-lab/conv-emotion)

---

### 🔷 2. MMGCN
> **MMGCN** serves as a **multimodal GCN baseline**. It builds a complete graph over modalities (text, audio, visual) and applies spectral GCN to learn inter-modal interactions.
- 🔗 **Paper** → [MMGCN (Hu et al., 2021)](https://arxiv.org/pdf/2109.06195.pdf)
- 💻 **Code** → [hujingwen6666/MMGCN](https://github.com/hujingwen6666/MMGCN)

---

### 🔷 3. MultiEMO-GCN
> I include **MultiEMO-GCN** as a **cross-modal attention-based baseline**. It focuses on hierarchical attention to fuse different modalities and addresses class imbalance using focal loss.
- 🔗 **Paper** → [MultiEMO (Shi et al., 2023)](https://arxiv.org/pdf/2305.15390.pdf)
- 💻 **Code** → [TaoShi1998/MultiEMO](https://github.com/TaoShi1998/MultiEMO)

---

### 🔷 4. TelME
> **TelME** introduces **cross-modal knowledge distillation**, where the text modality teaches audio and visual features. This model is used as a **knowledge-guided baseline** for fusion and robustness.
- 🔗 **Paper** → [TelME (Yun et al., NAACL 2024)](https://aclanthology.org/2024.naacl-main.8.pdf)
- 💻 **Code** → [yuntaeyang/TelME](https://github.com/yuntaeyang/TelME)

---

## 📁 Structure
- `data/`: Contains preprocessed MELD or IEMOCAP datasets
- `DialogueGCN/`, `MMGCN/`, `MultiEMO/`, `TelME/`: Baseline model codebases
- `scripts/`: My experimental pipelines and evaluation scripts

---

## 🚧 Work in Progress
Current work involves:
- Standardizing data format across baselines
- Unifying evaluation metrics
- Analyzing latent graph structures and modality contributions

---

## 📚 Citation
Please cite the original authors if you use any of these models. This repo is only for academic benchmarking.

