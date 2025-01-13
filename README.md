# License Plate Detection with YOLOv8 and SORT  

This project implements a license plate detection system using YOLOv8 for object detection, SORT for object tracking, and EasyOCR for optical character recognition (OCR). It detects vehicles, extracts license plates, and recognizes their text from video footage.  

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
   https://github.com/FahithKRM/License-Plate-Detection-System
   cd License-Plate-Detection-System
   ```
2. Install the required dependencies:  
   ```bash
   pip install -r requirements.txt
   ```
3. Download the YOLOv8 weights:
   - For vehicle detection: YOLOv8 COCO weights
   - For license plate detection: Custom-trained YOLOv8 weights (place in the weights/ folder).
  
## Directory Structure
license-plate-detection/
├── main.py                 # Core pipeline for detection and tracking
├── util.py                 # Helper functions (OCR, validation, formatting)
├── add_missing_data.py     # Interpolates missing tracking data
├── visualize.py            # visualize the data
├── models/                 # YOLOv8 model weights
├── results/                # Output CSV and annotated frames
├── requirements.txt        # Python dependencies
├── README.md               # Project documentation


