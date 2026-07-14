# Gesture-Based Text Creation and Recognition

A computer vision project developed during **Summer of Code (SoC) 2024** that enables intuitive human-computer interaction using hand gestures. The project features a Virtual Notepad for air writing and handwritten digit recognition, along with gesture-controlled applications such as brightness control, volume control, image drag-and-drop, and screen pause detection.

---

## Overview

This project explores real-time hand gesture recognition using **MediaPipe**, **OpenCV**, and **TensorFlow**. By tracking hand landmarks through a webcam, users can interact with their computer without traditional input devices.

The repository also includes assignments completed during the Summer of Code program, covering machine learning and deep learning fundamentals.

---

## Features

### Virtual Notepad

- Draw on a virtual canvas using hand gestures
- Multiple drawing colors
- Eraser functionality
- Save drawings
- Handwritten digit recognition using a CNN trained on the MNIST dataset
- Interactive toolbar

### Brightness Control

- Adjust system brightness using hand gestures

### Volume Control

- Control system volume using finger distance

### Gesture-based Drag and Drop

- Move an image on the screen using hand gestures

### Pause Detection

- Pause the application by showing four or more fingers

### Handwritten Digit Recognition

- Recognize digits drawn on the virtual canvas using a Convolutional Neural Network

---

## Tech Stack

| Category | Technologies |
|----------|--------------|
| Programming Language | Python |
| Computer Vision | OpenCV |
| Hand Tracking | MediaPipe |
| Deep Learning | TensorFlow, Keras |
| Numerical Computing | NumPy |
| System Control | WMI, Pycaw |

---

## Repository Structure

```text
.
├── Assignment1-Part1.ipynb
├── Assignment1-Part2.ipynb
├── Assignment2.ipynb
├── Assignment3-Part1.ipynb
├── Assignment3-Part2.ipynb
├── Assignment3-Part3.ipynb
├── Assignment3-Part4.ipynb
├── BrightnessHandGesture.ipynb
├── DragAndDrop.py
├── HandTrackingModule.py
├── MnistModel.ipynb
├── Pause.py
├── VirtualNotepad.py
├── cnnmodel/
└── headerImages/
```

---

## System Workflow

```text
Webcam
   │
   ▼
MediaPipe Hand Tracking
   │
   ▼
Hand Landmark Detection
   │
   ▼
Gesture Recognition
   │
   ├── Virtual Drawing
   ├── Erasing
   ├── Brightness Control
   ├── Volume Control
   ├── Drag and Drop
   └── Digit Recognition
```

---

## Installation

Clone the repository.

```bash
git clone https://github.com/akkshitha676/SoC-24-Gesture-Based-Text-Creation-and-Recognition.git
```

Move into the project directory.

```bash
cd SoC-24-Gesture-Based-Text-Creation-and-Recognition
```

Install the required dependencies.

```bash
pip install opencv-python mediapipe tensorflow numpy pycaw comtypes wmi
```

---

## How to Use

### Virtual Notepad

1. Run the application.
2. Allow access to your webcam.
3. Position your hand in front of the camera.
4. Use your index finger to draw on the virtual canvas.
5. Use selection mode to choose colors or tools.
6. Use the eraser to remove unwanted strokes.
7. Draw a handwritten digit and use the prediction option to recognize it.
8. Save your drawing if required.

### Brightness Control

1. Run the brightness control application.
2. Perform the designated pinch gesture.
3. Move your fingers closer or farther apart to decrease or increase screen brightness.

### Volume Control

1. Run the volume control application.
2. Adjust the distance between your thumb and index finger.
3. The system volume changes according to the detected finger distance.

### Drag and Drop

1. Launch the drag-and-drop application.
2. Select the object using the predefined gesture.
3. Move your hand to reposition the object on the screen.

### Pause Detection

1. Run the pause detection application.
2. Show four or more fingers to trigger the pause action.

---

## Running the Applications

Launch the Virtual Notepad.

```bash
python VirtualNotepad.py
```

Run the Drag and Drop application.

```bash
python DragAndDrop.py
```

Run Pause Detection.

```bash
python Pause.py
```

---

## Gesture Controls

| Gesture | Action |
|----------|--------|
| Index Finger | Draw |
| Two Fingers | Selection Mode |
| Eraser Gesture | Erase Drawing |
| Pinch Gesture | Brightness Control |
| Finger Distance | Volume Control |
| Grab Gesture | Drag and Drop |
| Four Fingers | Pause Screen |
| Predict Button | Recognize Handwritten Digit |

---

## Machine Learning

The handwritten digit recognition module uses a Convolutional Neural Network trained on the **MNIST** handwritten digit dataset.

Prediction pipeline:

1. Capture the drawing from the virtual canvas.
2. Convert the image to grayscale.
3. Resize the image to **28 × 28** pixels.
4. Normalize the pixel values.
5. Pass the processed image through the trained CNN.
6. Display the predicted digit.

---

## Learning Modules

This repository also contains assignments completed during the Summer of Code program.

### Assignment 1

- NumPy
- Pandas
- Matplotlib

### Assignment 2

- Activation Functions
  - ReLU
  - Sigmoid
  - Tanh
- Multi-Layer Perceptron

### Assignment 3

- Neural Networks
- Deep Learning Experiments
- Convolutional Neural Networks
- Model Training

---

## Future Improvements

- Multi-digit recognition
- Word-level handwriting recognition
- Undo and Redo functionality
- Shape recognition
- Custom gesture mapping
- Multi-user support
- Cloud deployment
- Cross-platform compatibility

---

If you found this project interesting or useful, consider giving the repository a star.
