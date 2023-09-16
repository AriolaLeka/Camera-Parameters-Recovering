# Camera Parameter Recovery from Images

This repository contains the code and materials for a project focused on recovering internal and external camera parameters from images. The objective is to estimate the camera calibration matrix (K), camera orientation (R), and the world coordinates of the camera (Ce) for two images, namely "house1.png" and "house2.png."

## Task Description

The project involves the following tasks:

1. **Image Coordinate Extraction**: Finding the image coordinates (xi) for 10 cardinal points marked in the image "house1.png." This can be achieved either through line detection using the Hough transform and intersection or manual extraction.

2. **Projection Matrix Reconstruction**: Reconstructing the projection matrix (P) using the Direct Linear Transform (DLT) algorithm. In this step, we may encounter a rank deficiency in the matrix A, but we will adapt the solution to ensure it works.

3. **Camera Parameter Estimation**: From the projection matrix P, we aim to recover:
   - Camera calibration matrix (K)
   - Camera orientation (R)
   - Non-homogeneous world coordinates of the camera (Ce)

## Getting Started

### Prerequisites

Ensure you have the following dependencies installed:

- [Python](https://www.python.org/)
- [NumPy](https://numpy.org/)
- [Matplotlib](https://matplotlib.org/)
- [Math](https://docs.python.org/3/library/math.html)

## Results
The estimated camera parameters (K, R, Ce) for both "house1.png" and "house2.png" can be found in the results/ directory. These results are based on the image coordinate extraction and DLT algorithm implementation.
 
## Acknowledgments
This project was done in collaboration with Shega Likaj and Francisco Amoros Cubells.
