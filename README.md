# Image Matching Algorithms for Multi-Temporal Satellite Images

## Overview
This repository presents a comparative study of feature-based image matching algorithms applied to multi-temporal satellite imagery. The project evaluates classical computer vision techniques under real-world remote sensing conditions such as scale variation, rotation, resolution differences, and temporal changes.

The study investigates the performance of SIFTE feature detectors combined with Brute Force and FLANN matchers. To improve robustness and reduce false correspondences, Gaussian filtering and RANSAC-based outlier rejection are applied. Experimental results are supported by a detailed technical report.

---

## Algorithms and Techniques

### Feature Detectors & Descriptors
- SIFT (Scale-Invariant Feature Transform)

### Matching Methods
- FLANN (Fast Library for Approximate Nearest Neighbors)

### Optimization and Post-Processing
- Gaussian Blur (noise reduction)
- RANSAC (robust homography estimation)
- Distance-based match filtering
- K-Means clustering for spatial analysis of matched keypoints

---

## Dataset
- Satellite images acquired from Google Earth
- Minimum 3-year temporal difference between image pairs
- Multiple spatial resolutions (including 4K and 8K images)
- Test scenarios include:
  - Rotation
  - Scale variation
  - Partial image matching
  - Multi-temporal urban changes

> Only sample images are included in this repository for demonstration purposes.

---

## Experimental Findings
- SIFT + FLANN + RANSAC provides the highest matching accuracy but has higher computational cost.
- Applying RANSAC significantly reduces false matches, particularly along edges and repetitive structures.
- K-Means clustering helps analyze the spatial consistency and distribution of matched keypoints.



