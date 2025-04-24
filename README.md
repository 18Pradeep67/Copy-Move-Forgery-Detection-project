# Copy-Move Forgery Detection

This project aims to detect copy-move forgeries in digital images using a deep learning (U-Net) approach and handcrafted techniques (CenSurE + FREAK + clustering, DFFT+DBSCAN ). It is designed for research and educational purposes.

---

### Features

- **U-Net-based Semantic Segmentation**  
  Deep learning model trained to generate pixel-wise binary masks identifying tampered regions.

- **CenSurE + FREAK Keypoint-Based Detection**  
  Handcrafted feature-based approach using CenSurE keypoints, FREAK descriptors, and clustering to highlight potential copy-move regions.

- **Support for CASIA 2.0 Dataset**  
  Prepares and processes images and corresponding ground truth masks from the CASIA v2.0 dataset.

- **Visualization Tools**  
  Side-by-side visualization of forged regions and ground truth masks for both detection pipelines.

---

## Techniques Used

- **U-Net** for semantic segmentation (PyTorch)
- **CenSurE (STAR)** keypoint detection (OpenCV)
- **FREAK** descriptors
- **k-NN matching** with Brute Force Matcher
- **DBSCAN / Agglomerative Clustering** for grouping matched keypoints
- **Matplotlib** for result visualization

---

