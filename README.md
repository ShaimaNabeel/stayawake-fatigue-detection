# StayAwake — Driver Fatigue Detection

StayAwake is a real-time driver fatigue detection system that classifies a driver's state as awake, drowsy, or sleepy using facial features and deep learning.

## Features

- Classifies driver state into awake, drowsy, and sleepy
- Fine-tuned ResNet18 image classification model
- Real-time face landmark detection using MediaPipe Face Mesh
- Eye Aspect Ratio (EAR) for eye-closure detection
- Mouth Aspect Ratio (MAR) for yawn detection
- Audio alerts for drowsiness and sleepiness
- Real-time OpenCV video display and recording

## Model and Training

The image classifier was built using a fine-tuned ResNet18 model.

- Data split: 80% training and 20% validation
- Optimizer: Adam
- Learning rate: 0.0001
- Image size: 224 × 224
- Data augmentation: horizontal flip, rotation, and color jitter
- Training and validation accuracy: approximately 98%

## Real-Time Detection Rules

- EAR below 0.20 for 2 seconds indicates sleepiness.
- MAR above 0.60 for 1.5 seconds indicates drowsiness.

## Tech Stack

- Python
- PyTorch
- ResNet18
- OpenCV
- MediaPipe
- Pygame
- NumPy

## Author

**Shaima Nabeel Albokhari**  
Computer Science Graduate | Data & AI
