# Image Enhancement and Segmentation Pipeline

##  Project Overview

This project implements a complete image processing pipeline for **road scene analysis** using image enhancement and segmentation techniques. The system processes input frames, enhances image quality, performs segmentation, and generates final detected outputs.

The pipeline is designed as part of the **Final Integration Program** requirement and demonstrates all intermediate and final processing stages.

---

##  Processing Pipeline

The system follows a structured pipeline:

Input Frames → Image Enhancement → Segmentation → Contour Detection → Final Output

### Key Stages:

1. **Input Frames**
2. **Grayscale Conversion**
3. **Blurring (Noise Reduction)**
4. **Contrast Enhancement**
5. **Thresholding (Segmentation)**
6. **Morphological Operations (Opening, Dilation)**
7. **Edge Detection**
8. **Contour Detection**
9. **Final Marked Output**

---

##  Project Structure

```
segmentation01/
│
├── Untitled-Copy2.ipynb          # Main implementation notebook
├── quantitative_results.csv     # Evaluation results
├── table_a_overall.csv          # Overall performance metrics
├── table_b_videowise.csv        # Video-wise results
│
├── ground_truth_masks/          # Ground truth segmentation masks
├── predicted_masks/             # Model predicted masks
│
├── output_member2/              # Full pipeline outputs (step-by-step)
│   ├── 1_input_frames/
│   ├── 2_gray_frames/
│   ├── 3_blur_frames/
│   ├── 4_blackhat_frames/
│   ├── 5_thresh_frames/
│   ├── 6_opening_frames/
│   ├── 7_dilation_frames/
│   ├── 8_edges_frames/
│   └── 9_contours_frames/
│
├── segmentation_results/        # Segmentation pipeline outputs (method 1)
├── segmentation_results1/       # Segmentation pipeline outputs (method 2)
│
├── road_member2_gaussian_contrast/
├── road2_member2_gaussian_contrast/
├── road_member3_sharpened/
```

---

##  Image Enhancement Techniques

The project applies several enhancement methods:

* Grayscale conversion
* Gaussian blur for noise reduction
* Blackhat transformation for contrast enhancement
* Gaussian contrast adjustment
* Image sharpening

These steps improve feature visibility before segmentation.

---

##  Segmentation Methods

Segmentation is performed using:

* Thresholding techniques
* Morphological operations (opening, dilation)
* Edge detection
* Contour extraction

Multiple segmentation pipelines are implemented and stored in:

* `segmentation_results/`
* `segmentation_results1/`

---

##  Evaluation

The project includes quantitative evaluation using:

* Ground truth masks (`ground_truth_masks/`)
* Predicted masks (`predicted_masks/`)
* CSV result files:

  * `quantitative_results.csv`
  * `table_a_overall.csv`
  * `table_b_videowise.csv`

---

##  How to Run

### Requirements:

* Python 3.x
* Jupyter Notebook

### Install dependencies:

```
pip install opencv-python numpy matplotlib
```

### Run the project:

1. Open:

```
Untitled-Copy2.ipynb
```

2. Run all cells step-by-step

---

##  Input

* Road video frames (already included in folders)

---

##  Output

The system generates:

* Enhanced frames
* Segmented masks
* Edge-detected frames
* Contour-marked outputs

All outputs are stored in structured folders inside:

* `output_member2/`
* `segmentation_results/`
* `segmentation_results1/`

---

## key Features

* Complete end-to-end processing pipeline
* Multiple segmentation approaches
* Intermediate step visualization
* Quantitative performance evaluation
* Organized output storage for reporting

---

##  Notes

* All intermediate processing stages are saved for analysis
* Multiple enhancement techniques are tested and compared
* Results are reproducible using the provided notebook

---
