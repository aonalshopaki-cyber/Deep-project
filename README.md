# Deep-project: Multimodal Crop Disease Classification

[cite_start]This repository contains the code for our submission to the **ICPR 2026 AgVision Kaggle Competition**: *Beyond Visible Spectrum: AI for Agriculture 2026*[cite: 6]. 

[cite_start]Our proposed model, **SEFusionNet**, is a dual-branch deep learning architecture designed to accurately classify crop health conditions (Healthy, Rust-infected, Other) by dynamically fusing high-dimensional hyperspectral (HS) data with multispectral (MS) and RGB imagery[cite: 7, 8, 56, 57].

## 🚀 Key Contributions
* [cite_start]**Dual-Branch Architecture**: Utilizes a `ConvNeXt-Small` backbone for 125-band hyperspectral data and an `EfficientNet-B2` backbone for 8-channel (MS + RGB) spatial data[cite: 8, 62, 66].
* [cite_start]**SE-Guided Feature Fusion**: Employs a Squeeze-and-Excitation (SE) attention mechanism to dynamically recalibrate the importance of each feature channel before the final classification head[cite: 9, 68].
* [cite_start]**Robust Optimization**: Trained using Focal Loss (to handle ambiguous edge cases) and a OneCycleLR scheduler with differential learning rates for backbones vs. classification heads[cite: 10, 84, 89, 91].

## ⚙️ Setup and Installation

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/aonalshopaki-cyber/Deep-project.git](https://github.com/aonalshopaki-cyber/Deep-project.git)
   cd Deep-project
