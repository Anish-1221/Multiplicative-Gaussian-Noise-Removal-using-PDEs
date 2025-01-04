# Multiplicative Gaussian Noise Removal using Partial Differential Equations (PDEs)

This repository implements a novel method for removing multiplicative Gaussian noise from images. The approach leverages **Partial Differential Equations (PDEs)** and various **activation functions**, focusing on kernel learning through explicit schemes with a Gray-Level Indicator (GLI) matrix.

## Project Details

Multiplicative noise poses significant challenges in image processing due to its nonlinear and signal-dependent characteristics. This project addresses these challenges by introducing a robust and stable denoising approach. Key highlights include:

- **Kernel Training**: Optimization of convolutional kernels using PDE-based methods to suppress noise while preserving important image details.
- **GLI Matrix**: Integration of a pixel intensity-based matrix to improve edge preservation and enhance denoising performance.
- **Activation Functions**: Experimentation with ReLU, Perona-Malik, and Charbonnier functions to evaluate their impact on performance.

### Methodology

The approach combines kernel learning with PDEs and activation functions to model and suppress multiplicative noise. Key steps include:
1. Initialization of kernels with techniques like Laplacian filters.
2. Optimization using methods like L-BFGS-B to minimize the error between noisy and clean images.
3. Application of the GLI matrix to refine the denoising process further.
4. Evaluation using Peak Signal-to-Noise Ratio (PSNR) and Structural Similarity Index Measure (SSIM).

### Results

Extensive experiments demonstrate that this method achieves:
- Enhanced PSNR and SSIM values.
- Better edge retention compared to traditional methods.
- Robust performance under varying noise levels.

### Applications

This denoising technique is applicable to:
- **Medical Imaging**: Enhancing diagnostic accuracy by reducing noise in scans.
- **Remote Sensing**: Improving the clarity of satellite imagery.
- **Surveillance**: Enhancing the visibility of images captured in noisy environments.

### Citation

If you use this repository in your research, please cite the accompanying paper:
```
Soumen Sinha, Anish Nethi, and Mahipal Jetta. 2023. Multiplicative Gaussian Noise Removal using Partial Differential Equations and Activation Functions: A Robust and Stable Approach. Proceedings of the 2023 International Conference on Algorithms, Computing, and Systems.
