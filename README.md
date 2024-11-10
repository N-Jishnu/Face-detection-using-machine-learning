# Face Detection and Tracking with Deep Learning and OpenCV

This project implements real-time face detection and bounding box localization using a convolutional neural network (CNN) built with TensorFlow and OpenCV. It leverages VGG16-based feature extraction for robust face recognition, augmented with Albumentations for data variability, and uses a custom bounding box regression model to accurately track faces in live video streams.

## Features

- **Image Collection and Labeling**: Collects images via OpenCV and annotates faces using LabelMe.
- **Data Augmentation**: Expands the dataset with Albumentations, enhancing model robustness.
- **Model Architecture**: Utilizes VGG16 for feature extraction with a two-head model—classification and bounding box regression.
- **Real-Time Face Tracking**: Detects and localizes faces on live video streams using OpenCV.

## Model Overview

The model is a custom-built face tracker that combines binary classification for face detection and bounding box regression for accurate localization. It includes:

- **Backbone**: VGG16 (pre-trained) for feature extraction.
- **Classification Head**: Identifies the presence of a face.
- **Bounding Box Head**: Predicts bounding box coordinates for face localization.

## Example Outputs

The model identifies faces in real-time video, drawing bounding boxes around detected faces with confidence scores.

## Repository Structure

```
FaceDetection/
├── data/                # Raw and augmented images with labels
├── notebooks/           # Optional Jupyter notebooks for data exploration
├── src/                 # Scripts for data collection, augmentation, training, and detection
├── requirements.txt     # Dependencies
└── README.md            # Documentation and setup instructions
```

## License

This project is licensed under the MIT License.
