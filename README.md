# Face Detection and Eye Detection using OpenCV

## Overview

This project demonstrates Face Detection and Eye Detection using OpenCV Haar Cascade Classifiers. The notebook detects human faces and eyes from images and highlights them using rectangular bounding boxes.

## Features

- Face Detection using Haar Cascade Classifier
- Eye Detection using Haar Cascade Classifier
- Works with grayscale and color images
- Visualization using Matplotlib
- Implemented in Python using OpenCV

## Technologies Used

- Python
- OpenCV
- NumPy
- Matplotlib
- Jupyter Notebook

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Face_Detection.git
cd Face_Detection
```

Install required packages:

```bash
pip install -r requirements.txt
```

## Required Libraries

```bash
pip install opencv-python
pip install numpy
pip install matplotlib
```

## Haar Cascade Files

OpenCV provides the required XML files:

```python
face_cascade = cv2.CascadeClassifier(
    cv2.data.haarcascades + 'haarcascade_frontalface_default.xml'
)

eye_cascade = cv2.CascadeClassifier('haarcascade_eye.xml')
```

## Face Detection Example

```python
faces = face_cascade.detectMultiScale(face_img,scaleFactor=1.2, minNeighbors=5) 
```

## Eye Detection Example

```python
eyes = eye_cascade.detectMultiScale(withglass) 
```

## Output

The detected faces and eyes are highlighted using rectangular bounding boxes.

### Face Detection

- Detects all visible faces in an image
- Draws rectangles around detected faces

### Eye Detection

- Detects eyes within the image
- Draws rectangles around detected eyes

## Applications

- Biometric Authentication
- Attendance Systems
- Surveillance Systems
- Human Computer Interaction
- Security Systems

## Future Enhancements

- Real-time Face Detection using Webcam
- Face Recognition using Deep Learning
- Smile Detection
- Mask Detection
- Object Tracking

## Author

**Charukesh S**

## License

This project is created for educational and academic purposes.
