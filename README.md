# Concrete Crack Segmentation Using Classical Digital Image Processing

## Course Information

University: Alamein International University

Faculty: Computer Science and Engineering

Course: Digital Image Processing

Course Code: CSE281

## Team Members and Roles

| Student Name | Student ID | Role |
|---|---|---|
| Nousiba Adel | 24100652 | Tech Lead & Data and Baseline Engineer |
| Nada Elshahat | 24100650 | Enhancement Engineer |
| Maryam Yasser | 24100639 | Restoration & Frequency Engineer |
| Mariam Emad | 25100637 | Segmentation Engineer |
| Yasmin Salah | 24100665 | Morphology & Evaluation Engineer |

## Project Overview

This project aims to develop a classical digital image processing pipeline for detecting and segmenting cracks in concrete surfaces and estimating the percentage of cracked surface area.

## Problem Statement

Manual inspection of concrete cracks can be time-consuming and susceptible to human error. Automatic crack detection is challenging due to low contrast, uneven illumination, noise, irregular crack shapes, and complex surface textures.

The proposed system applies classical digital image processing techniques to identify cracks, generate binary segmentation masks, and measure the affected surface area.

## Target Users

- Civil engineers.
- Structural inspectors.
- Infrastructure maintenance teams.

## Cost of Errors

Missing cracks may result in overlooking potential structural damage, while false detections may lead to unnecessary inspections and maintenance costs.

## Project Objectives

- Detect cracks in concrete surface images.
- Improve image contrast and visibility.
- Reduce image noise.
- Separate cracks from the background.
- Generate binary crack masks.
- Refine segmentation using morphological operations.
- Calculate the percentage of cracked surface area.
- Compare different image processing techniques.
- Evaluate performance against ground truth masks.

## Dataset

Dataset Name: Concrete Crack Segmentation Dataset

Source: Mendeley Data

Dataset URL: https://data.mendeley.com/datasets/jwsn7tfbrp/1

The dataset contains real-world concrete surface images and corresponding binary ground truth masks.

## Input

RGB concrete surface images.

Image dimensions, bit depth, data type, and intensity range will be verified during dataset analysis.

## Output

- Binary crack segmentation mask.
- Crack area in pixels.
- Crack area percentage.

## Primary Evaluation Metric

Intersection over Union (IoU).

IoU measures the overlap between the predicted crack mask and the ground truth mask relative to their combined area.

IoU = Intersection Area / Union Area

IoU is selected because it accounts for both missed cracks and incorrectly detected regions.

## Secondary Evaluation Metrics

- Mean Squared Error (MSE).
- Peak Signal-to-Noise Ratio (PSNR).
- Processing time.

MSE and PSNR will be used for image restoration experiments.

## Proposed Methodology

1. Dataset preparation.
2. Image analysis.
3. Baseline implementation.
4. Image enhancement.
5. Image restoration.
6. Frequency-domain processing.
7. Image segmentation.
8. Morphological refinement.
9. Crack area measurement.
10. Performance evaluation.

## Baseline Methods

Baseline 1: Fixed global thresholding with a threshold value of 127.

Baseline 2: Otsu thresholding followed by morphological opening using a 3 × 3 structuring element.

## Data Splitting

- Development Set: 70%.
- Test Set: 30%.

The development set will be used for experimentation and parameter tuning. The test set will be reserved for final evaluation.

## Project Scope

The project relies on classical digital image processing techniques without using machine learning or deep learning models.

## Tools and Technologies

- Python
- NumPy
- OpenCV
- SciPy
- scikit-image
- Matplotlib
- Google Colab
- GitHub

## Project Milestones

**Milestone 1:** Problem selection, dataset verification, primary metric selection, team role assignment, and repository preparation.

**Milestone 2:** Image analysis, data preparation, metric implementation, and baseline evaluation.

**Milestone 3:** Pipeline design and implementation.

**Milestone 4:** Experiments, parameter tuning, ablation studies, evaluation, and failure analysis.

**Final Submission:** GitHub Repository, Technical Report, Presentation, and Live Demo.

## Project Limitations

The proposed system is an academic digital image processing project intended to support visual inspection. It is not a substitute for professional structural assessment.

## Current Project Status

Milestone 1 – Project Preparation.

Dataset matching, licence verification, and image specifications are being reviewed before proceeding to Milestone 2.
