# Denoising of Speckled Cardiac Ultrasound Images Using Wavelet Transform

## Overview
This project focuses on denoising **Cardiac Ultrasound Images (CUI)** affected by speckle noise using **Wavelet Transform techniques** in MATLAB. The developed tool evaluates multiple wavelet mother functions, thresholding types (soft and hard), and decomposition levels to determine the optimal despeckling approach while preserving critical image details.

## Features
- Implements **five wavelet mother functions**:
  - Daubechies (db)
  - Symlets (sym)
  - Coiflets (coif)
  - Biorthogonal (bior)
  - Discrete Meyer (dmey)
- Supports **hard and soft thresholding** techniques.
- Analyzes images using key performance metrics:
  - **Peak Signal-to-Noise Ratio (PSNR)**
  - **Signal-to-Noise Ratio (SNR)**
  - **Structural Similarity Index (SSIM)**
- Provides a **Graphical User Interface (GUI)** for user interaction and threshold selection.
- Outputs the best wavelet configuration based on quantitative evaluation.

## Installation
### Requirements
Ensure you have the following software installed:
- **MATLAB** (R2020a or later recommended)
- Image Processing Toolbox
- Wavelet Toolbox

### Setup Instructions
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/denoising-cardiac-ultrasound.git
   ```
2. Open MATLAB and navigate to the project directory:
   ```matlab
   cd 'path_to_project'
   ```
3. Run the main script:
   ```matlab
   main_wavelet_denoising.m
   ```
4. Select an ultrasound image when prompted.
5. Choose between **soft and hard thresholding** from the GUI.
6. Review and compare denoised images with computed metrics.

## Usage
1. **Load an Image**: Select a speckled cardiac ultrasound image (.png, .jpg, .tif, etc.).
2. **Denoising Process**:
   - The script applies **Wavelet Transform decomposition** at levels 2-4.
   - Different **mother wavelets** are tested with both **soft and hard thresholding**.
   - Performance is assessed based on **PSNR, SNR, and SSIM**.
3. **Select Optimal Parameters**:
   - The GUI presents results from the **best wavelet configuration**.
   - Users can choose the most effective **thresholding method**.
4. **Results & Visualization**:
   - The best denoised image is displayed alongside the original.
   - Metrics and wavelet parameters are shown for comparison.

## Results
The tool determined that the **Biorthogonal wavelet (Bior6.8) with level-4 decomposition using soft thresholding** provided the best denoising performance while maintaining structural integrity. The **Discrete Meyer wavelet (dmey) with level-4 decomposition** was optimal for hard thresholding.

## File Structure
```
📂 denoising-cardiac-ultrasound
 ├── 📜 main_wavelet_denoising.m  # Main script with GUI implementation
 ├── 📜 wavelet_denoising.m       # Function for wavelet-based despeckling
 ├── 📜 metrics_computation.m     # Computes PSNR, SNR, and SSIM values
 ├── 📜 gui_selection.m           # GUI for threshold selection
 ├── 📂 sample_images             # Example cardiac ultrasound images
 ├── 📜 README.md                 # Project documentation
```

## References
1. Michailovich, O. V., & Tannenbaum, A. (2006). "Despeckling of medical ultrasound images." IEEE Transactions on Ultrasonics, Ferroelectrics, and Frequency Control, 53(1), 64-78. doi:10.1109/tuffc.2006.1588392.
2. Ndajah, P., et al. (2010). "SSIM image quality metric for denoised images." International Conference on Visualization, Imaging, and Simulation Proceedings, 53-57.

## Contributors
- **Safwan K. Sami** (Lead Developer)
- **Ahmed Khaleel**
- **Muhamed Rojba**
- **Ibrahim Rahman**

## License
This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
Special thanks to the **University of Illinois Chicago, Department of Bioengineering**, for providing guidance and resources for this project.

---
Feel free to contribute, suggest improvements, or report any issues in the repository!

