# Auto-Encoders Image Denoising Repository

## Overview

This repository contains an implementation of autoencoders for image denoising using RGB images. The autoencoder is designed in a split format, with separate encoder and decoder components. The denoising process involves introducing Gaussian noise to the original images and their corresponding codes in two different scenarios, and then mapping them back to denoised images.

## Specifications

1. **RGB Image Processing**
   - The autoencoder is designed to work with RGB images.

2. **Image Denoising Scenarios**
   - **Scenario 2.1:** Gaussian noise with a specified Mu & Sigma is added to the original images. This noisy input is fed into the encoder to generate a noisy code, which is then mapped back to the original images at the decoder (Noisy images -> Denoised images).
   - **Scenario 2.2:** Gaussian noise with the same Mu & Sigma as in 2.1 is added directly to the code. This noisy code is then mapped back to the same original images at the decoder (Noisy code -> Denoised images).

3. **Visual Comparison**
   - Visualize and compare the differences between results obtained from Scenario 2.1 and 2.2.

4. **Bonus Features**

   - **4.1 Image Denoising with PCA**
     - Utilized Principal Component Analysis (PCA) as an image denoiser and compared its results with the autoencoder. Performed both subjective and objective measures.
     - **Subjective Measure:** Visualized denoised images from both algorithms and state which algorithm yields better results.
     - **Objective Measure:** Computed the compression ratio for both algorithms (Reconstructed image / Original image).

   - **4.2 CNN as Encoder Input Layer**
     - Implemented a Convolutional Neural Network (CNN) as an input layer for the encoder, replacing the fully connected layer.

5. **Results Report**
   - Displayed all results, including denoised images, visual comparisons, and any additional metrics, in a comprehensive report.
