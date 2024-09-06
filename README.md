"Drivegaurd"-Driver Drowsiness Detection System

Overview

This project is a Driver Drowsiness Detection System that monitors a driver's eyes in real-time through a webcam and alerts the driver if drowsiness is detected. The system uses OpenCV for video processing, Keras for classifying eye states (open or closed), and a custom-trained deep learning model for the classification task.

Features

Real-time face and eye detection using OpenCV.
Eye state classification (open/closed) using a trained Keras model.
Drowsiness detection based on prolonged eye closure.
Alerts the driver when drowsiness is detected.

Table of Contents
Overview
Features
Installation
Usage
Dependencies
Model Training
Future Improvements
Contributing

Installation

To get started with the project, follow these steps:

Clone the repository:

git clone https://github.com/yourusername/driver-drowsiness-detection.git

Navigate to the project directory:

cd driver-drowsiness-detection

Create a virtual environment (optional but recommended):

python -m venv venv

source venv/bin/activate  # On Windows: venv\Scripts\activate

Install the required dependencies:

Usage

Run the drowsiness_detection.py file:

python drowsiness_detection.py

The system will activate the webcam and begin monitoring. If the driver’s eyes remain closed for too long, the system will raise an alert.

Dependencies

The project requires the following libraries:

Python 3.x
OpenCV: For real-time video capture and face/eye detection.
Keras: For loading and using the pre-trained deep learning model.
TensorFlow: Backend for Keras.
NumPy: For numerical operations.
dlib: For landmark detection (optional).
imutils: For easier image processing functions.

Model Training

The Keras model was trained on a dataset of eye images labeled as either open or closed. If you want to train the model yourself:
Gather or use an existing dataset of labeled images (open/closed eyes).

Use the provided train_model.py script to train the model:

python train_model.py
The model will be saved in the model/ directory as eye_state_model.h5.

Future Improvements
Implement head pose estimation to enhance detection accuracy.
Add yawning detection for a more comprehensive drowsiness assessment.
Optimize the model for mobile and edge devices.

Contributing
Contributions are welcome! Please submit a pull request or open an issue to discuss improvements or bugs.
