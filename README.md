# License Plate Recognition with Arabic Letters and Numbers

## Project Overview
This project focuses on developing a system for **automatic license plate recognition (ALPR)** that supports **Arabic letters and numbers**. The system utilizes **YOLOv1 (fine-tuned)** for plate detection and **EasyOCR** for optical character recognition (OCR). The objective is to create a robust and efficient model capable of recognizing Egyptian license plates.

## Features
- **Automatic detection** of license plates in images and video frames.
- **Recognition of Arabic letters and numbers** on Egyptian plates.
- **Deep learning-based approach** using **YOLOv1** for detection.
- **OCR processing** using **EasyOCR** for text extraction.
- **Fine-tuned model** for improved accuracy on Egyptian plates.

## Dataset
The dataset used for training includes images of Egyptian license plates annotated with bounding boxes and corresponding text labels. The dataset is preprocessed and augmented to improve model generalization.

## Technologies Used
- **YOLOv1** (You Only Look Once) for object detection
- **EasyOCR** for character recognition
- **Python** as the primary programming language
- **OpenCV** for image processing
- **TensorFlow/PyTorch** (if applicable for training YOLO)
- **Jupyter Notebook** for experimentation

## Installation
### Prerequisites
Ensure you have Python installed along with the required dependencies.

```bash
pip install opencv-python torch torchvision easyocr numpy matplotlib
```

### Clone the Repository
```bash
git clone <https://github.com/marawan-mogeb/egyptian-car-plates-yolov11-easyocr.git>
cd <project_directory>
```

## Usage
### Running the Model
1. **Load the trained YOLO model** for license plate detection.
2. **Pass an image or video frame** through the model.
3. **Extract the license plate region** and apply OCR for text recognition.

Example usage:
```python
import cv2
import easyocr

# Load image
image = cv2.imread('car.jpg')

# Run YOLO model for plate detection (Assuming model is loaded)
# Detect the plate and extract the region of interest (ROI)

# Run OCR on the extracted plate
reader = easyocr.Reader(['ar', 'en'])
text = reader.readtext(roi, detail=0)
print("Detected License Plate:", text)
```

## Model Training
If you need to train the model from scratch:
1. Prepare and annotate the dataset.
2. Fine-tune YOLOv1 on the dataset.
3. Evaluate and optimize performance.


## Contributors
- **Marawan Mogeb Alrahman Fouad**
- **Ahmed Mohamed Farrag**
- **Ahmed Mohamed Abbas**
- **Ahmed Salah**
- **Mohamed Hossam**


