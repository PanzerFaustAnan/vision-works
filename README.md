# Medical Image Registration & Segmentation — Research Notebooks

Research notebooks from my work as a Research Assistant (Feb 2025–Present) under **Dr. Tonmoy Hossain Dihan**, Postdoctoral Research Fellow, Harvard Medical School (remote collaboration). Organized to mirror the "Research Experience" section of my CV — each notebook here corresponds to a specific sub-project described there.

> These are research-in-progress notebooks, not polished final deliverables.

---

## 1. Generative Modeling & Vision–Language Models for Image Registration

Early pipeline validation for combining SigLIP-based vision encoders with VoxelMorph-style deformable registration — custom registration losses and displacement-field analysis, tested on paired-image data as a fast testbed before scaling to volumetric MRI. Uses `google/medsiglip-448` as the vision encoder.

📁 [`MedSigLip_+_VoxelMorph.ipynb`](./MedSigLip_+_VoxelMorph.ipynb)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1r77vcfLMmq1015wJym1f88S9O9NjcsJY?usp=sharing)

---

## 2. SynthSeg Pipeline Dissection & Quantitative Evaluation

Dissected each stage of the SynthSeg (Billot et al.) synthetic image generation pipeline from first principles using NumPy/SciPy — reparameterization trick, diffeomorphic elastic deformation via scaling-and-squaring — rather than treating the released code as a black box.

📁 [`SynthSeg_step_by_step_v3.ipynb`](./SynthSeg_step_by_step_v3.ipynb)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vxKs-QMnYOQjGWqMcS4Br54SFXbQPe_C?usp=sharing)

Quantitative comparison of SynthSeg (v1.0, v2.0) against FastSurfer on the Mindboggle-101 dataset (NKI-TRT-20 cohort, 20 subjects, manual DKT+aseg ground truth) — Dice, HD95, ASSD, and qualitative overlays.

📁 [`SynthSeg_v1_vs_v2_vs_FastSurfer_comparison_v2.ipynb`](./SynthSeg_v1_vs_v2_vs_FastSurfer_comparison_v2.ipynb)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19xyEA6nxiVUU8SMbd62IZ4UJVI4LhYDn?usp=sharing)

---

## Tech Stack

Python, PyTorch, TensorFlow/Keras, NumPy/SciPy, HuggingFace Transformers, FreeSurfer, SynthSeg, VoxelMorph, Google Colab (GPU)

---

## Notes

Next planned addition: cross-modality generalization evaluation (T1 vs. T2, HCP S1200), extending the SynthSeg-vs-FastSurfer comparison beyond T1-weighted MRI.
