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

### Setup  
1. Clone this repository:  
   ```bash
   https://github.com/FahithKRM/License-Plate-Detection-System.git
   cd License-Plate-Detection-System
   ```
   
2. Install the required dependencies:  
   ```bash
   pip install -r requirements.txt
   ```
   
3. Download the SORT files:
- Clone the SORT repository or download the required files from [SORT GitHub](https://github.com/abewley/sort).
- Place the SORT implementation files in the sort/ directory of your project.


4. YOLOv8 models are already included in the repository:
- For vehicle detection: YOLOv8 COCO models.
- For license plate detection: Custom-trained YOLOv8 weights located in the models/ folder.

Ensure Python 3.8 or above is installed. GPU is recommended for faster processing.

---
  
## Directory Structure
license-plate-detection/

![image](https://github.com/user-attachments/assets/cde735bc-2413-4796-b1e4-61720bf5554b)

![image](https://github.com/user-attachments/assets/6170cbaf-e7a0-4de7-a0a9-df901898d4a2)

---

## Run the Code
#### Input video Name is sample.mp4, Then can change the right name of the input files
- Run main.py with a sample video file to generate the test.csv file: 
   ``` bash
   python main.py
   ```
- Run the add_missing_data.py to interpolate missing values and smooth out the output for unmatched frames:
   ```bash
   python add_missing_data.py
   ```

- Finally run the visualize.py with the interpolated CSV file to generate a smooth and enhanced output for license plate detection:
   ```bash
   python visualize.py
   ```
   
---

## Results
- Output CSV: Includes bounding boxes, license plate text, and confidence scores.
- Annotated Frames: Video frames saved with vehicle and license plate annotations.

---
