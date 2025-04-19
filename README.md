# Automatic Number Plate Recognition (ANPR)

This project implements an **Automatic Number Plate Recognition (ANPR)** system using Python, YOLO, and EasyOCR. The system detects vehicles and their license plates in video frames and extracts text from the plates using Optical Character Recognition (OCR).

## Features

- **Vehicle Detection**: Detects vehicles in video frames using YOLOv8
- **License Plate Detection**: Identifies license plates using a pre-trained YOLO model
- **Text Extraction**: Extracts text from license plates using EasyOCR
- **Video Annotation**: Annotates video frames with bounding boxes and recognized text
- **Data Export**: Outputs results to CSV files for further analysis

## Demo Videos
- [Download Input Video](https://www.kaggle.com/datasets/nimishshandilya/car-number-plate-video?select=Traffic+Control+CCTV.mp4)
- [View Output Video](https://youtu.be/xYmm1-If3-0)


## Project Structure
Automatic-number-plate-recognition/  
**├── add_missing_data.py**: Script to handle missing data  
**├── license_plate_detector.pt**: Pre-trained YOLO model for license plate detection  
**├── main.py**: Main script for running the ANPR pipeline  
**├── out.mp4**: Output video with annotations  
**├── README.md**: Project description and usage instructions  
**├── test_interpolated.csv**: Interpolated test data  
**├── test.csv**: Output results in CSV format  
**├── util.py**: Utility functions for OCR and data processing  
**├── video.mp4**: Input video for processing  
**├── visualize.py**: Script for visualizing results on video  
**├── yolov8n.pt**: Pre-trained YOLOv8 model for vehicle detection  
**└── sort/**: SORT tracker implementation  
 **├── sort.py**: Multi-object tracking algorithm  
 **├── requirements.txt**: Dependencies for SORT  
 **└── data/**: Training data for SORT 

## Requirements
pip install -r requirements.txt

## Usage
Run the ANPR Pipeline: Execute the main script to process the input video and generate results:
python main.py

## Visualize Results: 
Use the visualize.py script to annotate the video with bounding boxes and license plate text:
python visualize.py

## Key Scripts
**main.py**: Main entry point for the ANPR pipeline.

**visualize.py**: Annotates video frames with detection results.

**util.py**: Contains helper functions for OCR, formatting, and data export.

## Pre-trained Models
**yolov8n.pt**: YOLOv8 model for vehicle detection.

**license_plate_detector.pt**: YOLOv8 model for license plate detection.
