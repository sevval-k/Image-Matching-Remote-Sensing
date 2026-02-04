This project focuses on feature-based image matching techniques applied to multi-temporal satellite images.
The main goal is to analyze and compare the performance of classical computer vision algorithms under scale, rotation, resolution, and temporal changes commonly encountered in remote sensing data.

The study evaluates different feature detectors, matchers, and optimization techniques, supported by experimental results and a detailed technical report.

Algorithms Used

Feature Detectors & Descriptors

SIFT (Scale-Invariant Feature Transform)



Matching Techniques

FLANN (Fast Library for Approximate Nearest Neighbors)

Optimization & Filtering

Gaussian Blur (Noise Reduction)

RANSAC (Outlier Removal & Robust Homography Estimation)

Spatial Analysis

K-Means Clustering applied to matched keypoints

Dataset

Satellite images obtained from Google Earth

Images captured at least 3 years apart

Different resolutions (4K, 8K)

Tests include:

Rotation

Scale variation

Partial image matching

Temporal changes

Sample images are provided for demonstration purposes.

Key Findings

SIFT + FLANN + RANSAC provides the highest matching accuracy but has higher computational cost.


Applying RANSAC significantly reduces false matches, especially along edges and repetitive patterns.

