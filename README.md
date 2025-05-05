# Topic: Morphological Image Processing
## Morphological Image Processing – Fingerprint Cleaning
Morphological image processing involves operations that process images based on shapes. It is primarily used for the analysis of binary images but can be extended to grayscale images. These techniques are often used to:
Remove noise
Fill holes
Extract or enhance structures
Perform shape analysis
Improve results of edge-based or threshold-based segmentation

## Problem Statement:
The goal of this project is to clean and enhance fingerprint images using morphological image processing techniques. Fingerprint images often contain noise, smudges, and broken ridge lines that interfere with biometric recognition. This project uses digital image processing (DIP) techniques to denoise and clarify fingerprint patterns for better feature extraction and analysis.

## Techniques & Program Flow
### 1. Original Image Loading
Input: Raw fingerprint image (grayscale).
Purpose: Acts as the base for preprocessing and enhancement.

### 2. Gaussian Blurring
Technique: Gaussian filter with a (5,5) kernel.
Purpose: Reduces high-frequency noise while preserving ridge structures.

### 3. Adaptive Thresholding
Technique: Adaptive Gaussian Thresholding.
Purpose: Converts the image into a binary format for easier segmentation.

### 4. Morphological Opening
Technique: Erosion followed by Dilation (OpenCV).
Purpose: Removes small white noise from the background.

### 5. Morphological Closing
Technique: Dilation followed by Erosion.
Purpose: Fills small gaps and connects broken ridges in the fingerprint.

### 6. Final Processed Image
Combination: Cleaned, binarized, and (optionally) skeletonized fingerprint image.
Purpose: Suitable for feature extraction like minutiae detection or pattern matching.

### 7. Overlay and Visualization
Technique: Matplotlib subplots.
Purpose: Visualizes the transformation at each stage for analysis and comparison

## Technologies Used
##### Python 3.x
##### OpenCV
##### NumPy
##### Matplotlib
##### scikit-learn
##### scikit-image

# Team Details
####  Team Members       USN
####  Ranjith            4SO22CD038
####  Sudhanva Patil     4SO22CD055
####  Dilip S Angadi     4SO23CD401
