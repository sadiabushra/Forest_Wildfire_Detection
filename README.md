# Forest Wildfire Detection

**An Explainable Deep Learning Framework for Forest Wildfire Classification Using Custom CNNs and Transfer Learning**

Sadia Hossain Bushra, Sayada Zakia Afrinee, Ayan Chatterjee, Vimala Nunavath
University of South-Eastern Norway (USN) · NILU

Presented at **ICT-DM 2026** (online, 9 November 2026).

## Contents

| Path | Description |
|---|---|
| [`paper/ICT-DM2026_Explainable_Wildfire_Classification_Paper.pdf`](paper/ICT-DM2026_Explainable_Wildfire_Classification_Paper.pdf) | Camera-ready paper |
| [`presentation/ICT-DM2026_Wildfire_Presentation.pptx`](presentation/ICT-DM2026_Wildfire_Presentation.pptx) | Conference presentation slides |
| [`Forest_Wildfire_Detection_CNN_final.ipynb`](Forest_Wildfire_Detection_CNN_final.ipynb) | Notebook with the full pipeline (preprocessing, training, evaluation, saliency maps) |

## Overview

A controlled benchmark of five models for binary fire / non-fire image classification, using one dataset, one preprocessing pipeline and one set of metrics:

- Custom CNN tuned with Keras Tuner (trained with Adam and with SGD)
- MobileNetV2, ResNet50V2 and EfficientNetB3 (transfer learning)

The study also includes an augmentation ablation and gradient-based saliency maps.

**Key results (50-image test set):** ResNet50V2 reached 98% accuracy; the custom CNN reached 96% with about 50× fewer parameters, and the two are statistically tied (95% Wilson intervals). Geometric + photometric augmentation improved accuracy by 8 points.

## Dataset

Kaggle "Forest Fire Images" by M. S. Prasad.

## Contact

sadia.h.bushra@usn.no · saafr7491@usn.no · ayan@nilu.no · vimala.nunavath@usn.no
