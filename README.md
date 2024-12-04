Face Mask Detection System
This repository contains a Face Mask Detection System built using a Convolutional Neural Network (CNN) architecture with the MobileNetV2 pre-trained model. This system detects whether a person is wearing a face mask or not in real-time.

Overview
The system uses a MobileNetV2 backbone for feature extraction, fine-tuned on a dataset of face images with and without masks. It can process images or video streams and classify faces into two categories:

With Mask
Without Mask
Features
Efficient and lightweight architecture using MobileNetV2.
Real-time face detection and mask classification.
High accuracy on test datasets.
Compatible with webcam, IP cameras, or video files.
Dataset
The dataset used includes face images with and without masks, preprocessed to be compatible with the MobileNetV2 model.
Source: Public datasets like Kaggle Face Mask Dataset.
Getting Started
Prerequisites
Python 3.8+
Install the required libraries:
bash
Copy code
pip install -r requirements.txt
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/face-mask-detection.git
cd face-mask-detection
Download the MobileNetV2 weights (if not included). Use TensorFlow or Keras to automatically load the pre-trained model:

python
Copy code
from tensorflow.keras.applications import MobileNetV2
Usage
Run the detection script on images:

bash
Copy code
python detect_mask_image.py --image path/to/image.jpg
Run the detection script on a webcam feed:

bash
Copy code
python detect_mask_video.py
Model Architecture
The system uses the MobileNetV2 architecture with the following modifications:

Final dense layers fine-tuned on the face mask dataset.
Output layer with softmax activation for binary classification.
Project Structure
bash
Copy code
face-mask-detection/
│
├── dataset/                # Dataset folder (images with/without masks)
├── detect_mask_image.py    # Script to run detection on images
├── detect_mask_video.py    # Script to run detection on video feeds
├── model/                  # Folder containing the trained model
├── requirements.txt        # List of dependencies
├── README.md               # Project README file
└── utils.py                # Utility functions for preprocessing and inference
Results
Training Accuracy: ~95%
Test Accuracy: ~92%
Acknowledgments
Original backbone architecture: MobileNetV2
Dataset: Public datasets from Kaggle and other sources.
License
This project is licensed under the MIT License. Please acknowledge the original authors where applicable.

Contact
For any queries, feel free to reach out:

Name: Praveen Kumar Sahoo
