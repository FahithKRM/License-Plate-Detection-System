# License Plate Detection with YOLOv8 and SORT  

This project implements a license plate detection system using YOLOv8 for object detection, SORT for object tracking, and EasyOCR for optical character recognition (OCR). It detects vehicles, extracts license plates, and recognizes their text from video footage.  

---

## Table of Contents  
- [Features](#features)  
- [Technologies Used](#technologies-used)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Directory Structure](#directory-structure)  
- [Results](#results)  
- [Future Improvements](#future-improvements)  
- [License](#license)  

---

## Features  
- Detects vehicles (cars, trucks, buses) in video frames using YOLOv8.  
- Tracks detected vehicles across frames with SORT.  
- Identifies license plates within vehicle bounding boxes.  
- Extracts text from license plates using EasyOCR.  
- Logs results, including bounding boxes, license plate text, and confidence scores, in a CSV file.  

---

## Technologies Used  
- **YOLOv8**: For vehicle and license plate detection.  
- **SORT**: For real-time object tracking.  
- **EasyOCR**: For extracting license plate text.  
- **OpenCV**: For video frame processing.  
- **NumPy**: For numerical computations.  
- **Pandas**: For structured result logging in CSV format.  

---

## Installation  

### Prerequisites  
- Python 3.8 or above  
- A GPU (recommended for YOLOv8 inference)  

### Setup  
1. Clone this repository:  
   ```bash
   git clone https://github.com/yourusername/license-plate-detection.git
   cd license-plate-detection
