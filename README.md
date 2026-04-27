# Road Damage Detection – Integrated Pipeline
### ICT2403 – Graphics and Image Processing | Submission 04

---

## Overview

This program integrates the full road damage detection pipeline developed across all three team members:

| Module | Damage Type | Member | Method |
|--------|-------------|--------|--------|
| `segment_linear_cracks()` | Linear / longitudinal cracks | Member 1 | Canny edge detection + morphological closing |
| `segment_alligator_cracks()` | Alligator (fatigue) cracks | Member 2 | Black-Hat transform + density filtering |
| `segment_potholes()` | Potholes | Member 3 | Inverse binary threshold + contour area filter |

---

## Folder Structure
SUBMISSION04_GROUP_NAME_25
│
├── .ipynb_checkpoints/
├── output_member2/
├── road2_gaussian_contrast_mem2/
├── road_member2_gaussian_contrast/
├── road_member3_sharpened/
├── segmentation_results/
│
├── member1.ipynb
├── member2.ipynb
├── member3.ipynb
└── README.md      

## Output Description

| Folder | Contents |
|--------|----------|
| `enhanced_frames/` | One enhanced frame per input (Gaussian blur + contrast stretch) |
| `member1_cracks/` | `edges_*.jpg`, `morph_*.jpg`, `result_*.jpg` (green bounding boxes) |
| `member2_alligator/` | `blackhat_*.jpg`, `connect_*.jpg`, `result_*.jpg` (red bounding boxes) |
| `member3_potholes/` | `thresh_*.jpg`, `mask_*.jpg`, `result_*.jpg` (blue bounding boxes) |
| `final_marked_outputs/` | `final_*.jpg` – all detections overlaid on one frame |

**Colour coding in final output:**

- 🟩 **Green** = Linear Crack (Member 1)
- 🟥 **Red** = Alligator Crack (Member 2)
- 🟦 **Blue** = Pothole (Member 3)

  ---

## Team Contributions

| Member | Responsibility | Method |
|--------|---------------|--------|
| Member 1 | Linear crack segmentation | Canny + morphological closing |
| Member 2 | Alligator crack segmentation | Black-Hat + density filter |
| Member 3 | Pothole segmentation | Inverse threshold + contour filtering |
| Member 4 | Documentation | Documenting |

