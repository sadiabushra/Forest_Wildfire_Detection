# Forest Wildfire Detection

**An Explainable Deep Learning Framework for Forest Wildfire Classification Using Custom CNNs and Transfer Learning**

Sadia Hossain Bushra, Sayada Zakia Afrinee, Ayan Chatterjee, Vimala Nunavath
University of South-Eastern Norway (USN) · NILU

Presented at **ICT-DM 2026** (online, 9 November 2026).

> **Copyright notice:** © 2026 IEEE. Personal use of this material is permitted. Permission from IEEE must be obtained for all other uses, in any current or future media, including reprinting/republishing this material for advertising or promotional purposes, creating new collective works, for resale or redistribution to servers or lists, or reuse of any copyrighted component of this work in other works.
>
> The PDF in this repository is the **accepted version** of the paper. The final published version will be available on IEEE Xplore (link and DOI will be added here once published).

## Contents

| Path | Description |
|---|---|
| [`paper/ICT-DM2026_Explainable_Wildfire_Classification_Paper.pdf`](paper/ICT-DM2026_Explainable_Wildfire_Classification_Paper.pdf) | Accepted version of the paper (IEEE copyright notice on page 1) |
| [`presentation/ICT-DM2026_Wildfire_Presentation.pptx`](presentation/ICT-DM2026_Wildfire_Presentation.pptx) | Conference presentation slides |
| [`Forest_Wildfire_Detection_CNN_final.ipynb`](Forest_Wildfire_Detection_CNN_final.ipynb) | Notebook with the full pipeline (preprocessing, training, evaluation, saliency maps) |

## Overview

A controlled benchmark of five models for binary fire / non-fire image classification, using one dataset, one preprocessing pipeline and one set of metrics:

- Custom CNN tuned with Keras Tuner (trained with Adam and with SGD)
- MobileNetV2, ResNet50V2 and EfficientNetB3 (transfer learning)

The study also includes an augmentation ablation and gradient-based saliency maps.

**Key results (50-image test set):** ResNet50V2 reached 98% accuracy; the custom CNN reached 96% with about 50× fewer parameters, and the two are statistically tied (95% Wilson intervals). Geometric + photometric augmentation improved accuracy by 8 points.

## Dataset

**Source:** [Forest Fire Images](https://www.kaggle.com/datasets/mohnishsaiprasad/forest-fire-images) on Kaggle, published by Mohnish Sai Prasad (accessed 5 March 2026).

- 2 classes: **Fire** and **Non-Fire**
- 5,000 training images (2,500 per class) and a separate test set of 50 images (25 per class), as provided by the publisher
- Images from diverse real-world settings: dense forests, open vegetation and woodland near urban areas, with varied fire intensity, smoke, lighting and weather
- 389 corrupted (undecodable) files removed → **4,611** clean training images (2,112 Fire, 2,499 Non-Fire), split 80/20 stratified into 3,689 train / 922 validation

The dataset is not included in this repository. Download it from Kaggle and follow the dataset's licence terms.

Citation:

> Prasad, M.S.: Forest Fire Images. Kaggle (accessed: 5 March 2026). https://www.kaggle.com/datasets/mohnishsaiprasad/forest-fire-images

## Contact

sadia.h.bushra@usn.no · saafr7491@usn.no · ayan@nilu.no · vimala.nunavath@usn.no
