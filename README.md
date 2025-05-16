# Deepfake Video Preprocessing

A modular video preprocessing pipeline designed for preparing video data for deepfake detection tasks.
This pipeline extracts frames from videos, detects and crops faces, applies grayscale and resizing transformations,
and includes temporal and compression artifact visualizations.

---

# Project Description

This project supports the preprocessing of deepfake datasets such as FaceForensics++ (https://www.kaggle.com/datasets/xdxd003/ff-c23) by:
- Extracting raw frames from `.mp4` videos
- Detecting and cropping faces from each frame
- Converting face crops to grayscale
- Resizing face images to a uniform input size
- Generating plots to analyze temporal inconsistencies and compression artifacts
- 
---

# Project Structure
├── faces/ # Cropped face images
├── faces_grayscale/ # Grayscale face images
├── faces_resized/ # Resized face images 
├── frames/ # Raw extracted video frames
├── graphs/ # Temporal and compression artifact plots
├── main.ipynb # Full Colab notebook with processing pipeline
├── requirements.txt # Required Python packages
└── README.md # Project documentation

# How to Use It
1. Clone the Repository or Upload to Google Colab
2. Install Required Libraries
3. Upload Videos
4. Run the Pipeline

# Visual Outputs
Frames, faces, grayscale faces, temporal Inconsistencies and compression artifact graphs

# Requirements
| Library         | Purpose                                                         |
| --------------- | --------------------------------------------------------------- |
| `opencv-python` | For reading videos, extracting frames, image processing         |
| `matplotlib`    | For generating temporal and compression artifact plots          |
| `numpy`         | Core numerical operations on image arrays                       |
| `dlib`          | Face detection and landmark extraction                          |
| `imutils`       | Convenience functions for resizing, rotating, drawing on images |
| `scikit-image`  | (Optional) Additional image processing, e.g., FFT or filters    |
| `tqdm`          | Progress bars for loops (e.g., processing videos or frames)     |

# Using the requirements.txt
pip install -r requirements.txt


                   

