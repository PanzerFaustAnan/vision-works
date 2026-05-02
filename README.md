# Generative Modeling & Representation Learning Experiments

This repository contains a collection of ongoing research experiments focused on **representation learning, generative modeling, and visual understanding**. The work primarily explores Variational Autoencoders (VAEs), Conditional VAEs (CVAEs), and their extensions toward invariant learning and multimodal vision systems.

> Note: These are **research-in-progress notebooks** and do not represent final results.

---

## Research Areas

### 1. CVAE Optimization (Posterior Collapse Mitigation)
- Implementation of Conditional Variational Autoencoder (CVAE)
- Focus on improving latent space utilization
- Custom loss with **β-weighted KL divergence**
- Experiments with long training schedules to stabilize learning

📁 [CVAE_KLD_Optimization.ipynb](./CVAE_KLD_Optimization.ipynb)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PanzerFaustAnan/vision-works/blob/main/CVAE_KLD_Optimization.ipynb)

---

### 2. Learning Invariances in Visual Representations
- Study of how neural networks learn invariances under:
  - Rotation  
  - Translation  
  - Scaling  
  - Shearing  
- Conducted on **MNIST dataset**
- Custom CNN architecture with controlled data sampling
- Evaluation using classification metrics (accuracy, F1, etc.)

📁 [learning_Invariances_MNIST.ipynb](./learning_Invariances_MNIST.ipynb)

---

### 3. MedSigLIP + Deformable Image Registration
- Experimental integration of:
  - **SigLIP-based vision encoders**
  - **VoxelMorph-style deformable registration**
- Pairwise image alignment using learned transformations
- Custom registration losses and displacement analysis
- Early exploration toward **medical image alignment with representation learning**

📁 [MedSigLip_+_VoxelMorph.ipynb](./MedSigLip_+_VoxelMorph.ipynb)

---

## Tech Stack
- Python
- PyTorch
- Hugging Face Transformers (SigLIP)
- Torchvision
- NumPy, Matplotlib
- Scikit-learn

---

## Notes

These notebooks serve as **prototypes and experimental logs**.  
Future work includes:
- Extending CVAE applications
- Deeper study of covariance-aware representations
- Integration with Vision-Language Models (e.g., CLIP, SAM-style systems)

---
