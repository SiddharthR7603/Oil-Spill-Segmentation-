
---

# Oil Spill Segmentation for RGB Images

This project focuses on segmenting oil spills in RGB images using deep learning techniques. The main goal is to accurately identify and visualize oil and water regions in RGB images, differentiating them from other objects. This README provides detailed information on how to set up and run the project using the provided Jupyter Notebook and datasets.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Datasets](#datasets)
3. [Requirements](#requirements)
4. [Installation and Setup](#installation-and-setup)
5. [Usage Instructions](#usage-instructions)
6. [Results](#results)
7. [Troubleshooting](#troubleshooting)
8. [Acknowledgments](#acknowledgments)

## Project Overview

There are several existing oil spill segmentation projects that focus on satellite images. However, this project specifically targets RGB images, making it suitable for scenarios where satellite imagery is unavailable or where high-resolution RGB images are preferred. The segmentation results display oil in orange, water in blue, and other objects in grey.

## Datasets

The project utilizes two datasets for segmentation tasks:

1. **Shadow Dataset**:
   - Images Directory: `/shadow-dataset/shadow-images/`
   - Masks Directory: `/shadow-dataset/shadow-masks/`

2. **Brightdark Dataset**:
   - Images Directory: `/brightdark-dataset/brightdark-images/`
   - Masks Directory: `/brightdark-dataset/brightdark-masks/`

Please ensure the datasets are properly organized before running the Jupyter Notebook.

## Requirements

To run this project, you need the following dependencies:
- Python 3.x
- Jupyter Notebook or Jupyter Lab
- Required Python Libraries:
  - OpenCV
  - NumPy
  - Matplotlib
  - Google Colab (for using Google Drive if applicable)

You can install the required libraries using:
```bash
pip install opencv-python numpy matplotlib
```

## Installation and Setup

1. **Clone the Repository**:
   Download or clone this repository to your local machine.

2. **Upload Datasets**:
   Make sure to upload the datasets (`shadow-dataset` and `brightdark-dataset`) to your Google Drive or local directory where the Jupyter Notebook will be able to access them.

3. **Open Jupyter Notebook**:
   Open the provided `.ipynb` file in Jupyter Notebook or Jupyter Lab to begin.

## Usage Instructions

1. **Mount Google Drive (if using Colab)**:
   If you are using Google Colab, ensure that you mount your Google Drive to access the datasets by running the following code:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```

2. **Run the Notebook**:
   Follow the steps in the Jupyter Notebook to process the images and masks for oil spill segmentation.

3. **Visualize Results**:
   The segmentation output will display oil in orange, water in blue, and other objects in grey.

4. **Save Results**:
   The processed images will be saved in the specified output directories.

## Results

The segmentation results demonstrate clear differentiation between oil and water regions in RGB images. Below are the color representations used in the output images:
- **Oil**: Orange
- **Water**: Blue
- **Other Objects**: Grey

## Troubleshooting

- **Issue**: The segmentation colors do not appear as expected.
  - **Solution**: Verify that the mask values in your dataset match the expected values (e.g., oil should be mapped to a specific grayscale value like 51).

- **Issue**: Cannot access datasets or images.
  - **Solution**: Ensure that your datasets are properly linked in the notebook and that the paths are correct.

## Acknowledgments

This project was developed using deep learning techniques to differentiate oil spills from other regions in RGB images. We would like to thank the community and online resources for their support.
