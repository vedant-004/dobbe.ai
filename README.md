# dobbe.ai
Data Science Intern Assignment
Problem Understanding
Dental IOPA X-rays vary greatly in quality due to different acquisition setups. This affects AI model performance. The goal is to build an adaptive preprocessing pipeline that adjusts contrast, sharpness, and noise reduction based on image-specific quality metrics.

Dataset
Format: DICOM (.dcm) images
Variations: brightness, contrast, sharpness, noise
Metadata: Includes pixel spacing, modality, etc.

Static Pipeline:
Histogram equalization
Gaussian denoising
Fixed sharpening


Adaptive Pipeline:
Uses image metrics to decide:
CLAHE for low contrast
Denoising for high noise
Sharpening for low sharpness

Evaluation
PSNR and SSIM used for comparison

Visual and numeric results show improvement
