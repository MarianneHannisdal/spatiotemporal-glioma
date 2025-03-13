# spatiotemporal-glioma

Image processing pipeline for analyzing grade 4 glioma recurrence patterns using deep learning segmentation of mpMRI data and migration distance quantification

## Overview

This repository contains the code used in our study "Spatial-temporal recurrence patterns of grade 4 glioma using deep learning integrated mpMRI and molecular pathology: a multi-centre longitudinal study."

This codebase implements a comprehensive pipeline for analyzing spatial-temporal recurrence patterns in grade 4 gliomas using deep learning-based segmentation of multi-parametric MRI (mpMRI) data. It integrates volumetric tumor segmentation, anatomical brain mapping, and migration distance quantification to identify predictors of tumor progression and survival outcomes.

## Features

- **Deep Learning Segmentation**: Utilizes pre-trained nnU-Net for automated segmentation of tumor compartments (contrast-enhancing, non-enhancing, and necrotic core)
- **Anatomical Brain Mapping**: Implements SynthSeg+ for robust anatomical mapping across brain regions
- **Inter-timepoint Registration**: Performs registration between primary and recurrent tumor MRIs using ANTs
- **Migration Distance Analysis**: Calculates Hausdorff Distance 95 (HD95) metrics between tumor boundaries

## Key Findings

Our analysis demonstrated:
1. The CEcore/NE volume ratio (≤0.324) as a novel imaging biomarker that independently predicts improved overall survival
2. MGMT methylation status significantly influences age-dependent tumor progression patterns
3. Higher migration distances correlate with longer time to progression, challenging traditional "go or grow" hypotheses
4. Distinct anatomical migration probabilities 

## Requirements

- Python 3.11+
- PyTorch
- ANTs
- nnU-Net
- SynthSeg+
- Additional dependencies listed in requirements.txt

## Citation

If you use this code in your research, please cite:
Hannisdal MH, Lundervold A, Goplen D, et al. Spatial-temporal recurrence patterns of grade 4 glioma using
deep learning integrated mpMRI and molecular pathology: a multi-centre longitudinal study. 2025.

## License

MIT License

## Acknowledgments

This research was funded by Helse Vest, The Norwegian Cancer Society (grant # 190170), and KLINBEFORSK.
