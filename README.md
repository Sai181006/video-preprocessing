# Deepfake Video Preprocessing
What is Video Preprocessing?
A systematic process for preparing video data for deepfake detection. This method involves several steps to transform raw videos into a standard format suitable for computer analysis.

The key stages of this process are:

1. Frame Separation: Dividing videos into individual image snapshots.
2. Face Identification and Isolation: Automatically locating and extracting face regions from each snapshot.
3. Grayscale Conversion and Size Standardization: Converting facial images to black and white and adjusting them to a uniform size.
4. Visual Representation of Motion and Compression Issues: Generating visual aids to understand movement within the video and distortions caused by video saving methods.
   
The purpose of this structured preparation is to extract relevant visual and motion details, while making sure all video data is consistent. This helps improve the accuracy and reliability of computer systems designed to detect deepfake videos.

---

# Project Description

This project supports the preprocessing of deepfake datasets such as FaceForensics++ (https://www.kaggle.com/datasets/xdxd003/ff-c23) by:
- Extracting raw frames from `.mp4` videos
- Detecting and cropping faces from each frame
- Converting face crops to grayscale
- Resizing face images to a uniform input size
- Generating plots to analyze temporal inconsistencies and compression artifacts
  
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


                   

