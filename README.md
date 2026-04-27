# Face Recognition Attendance System

## Overview
This project is an automated attendance system that uses facial recognition to identify individuals and mark their attendance. It is implemented using Python with OpenCV and the face_recognition library and is designed to run in Google Colab.

## Features
- Face detection and recognition  
- Automatic encoding of registered faces  
- Attendance marking with date and time  
- Duplicate entry prevention within a session  
- Image upload and batch processing  
- Webcam snapshot capture in Google Colab  
- CSV export of attendance records  

## Technologies Used
- Python  
- OpenCV  
- face_recognition  
- NumPy  
- Pandas  
- Google Colab  

## Project Structure
known_faces/            - Stores registered face images  
test_images/            - Stores input images for testing  
attendance_records/     - Stores generated CSV attendance files  
main.ipynb              - Main project notebook  
README.md               - Project documentation  

## Installation
Run the following commands in Google Colab:

```python
!pip install face_recognition
!pip install opencv-python-headless
!pip install pandas
!pip install Pillow
```

## Usage

### Register Faces
Upload images into the known_faces/ folder.  
Each file name should be the person's name.

Example:
```python
nausheen.jpg
```

### Encode Faces
The system automatically encodes all uploaded images.

### Capture or Upload Image
- Upload an image  
- Or capture a webcam snapshot in Colab  

### Run Recognition
The system detects faces, compares with known faces, and marks attendance.

### Save Attendance
Attendance is stored in:
attendance_records/

File format:
attendance_YYYY-MM-DD_HH-MM-SS.csv

## How It Works
1. Load and encode known face images  
2. Capture or upload an image  
3. Detect faces in the image  
4. Compare faces with stored encodings  
5. Recognize and mark attendance  
6. Save attendance with timestamp  
7. Export as CSV  

## Limitations
- Google Colab does not support real-time webcam streaming  
- Webcam works only for single image capture  
- Accuracy depends on lighting and image quality  

## Future Improvements
- Real-time webcam detection in local system  
- Web interface using Flask or Streamlit  
- Database integration  
- Improved accuracy with deep learning models  

## output
<img width="1179" height="656" alt="image" src="https://github.com/user-attachments/assets/af3cd279-46ad-4e00-a2b0-08ef1a0892e9" />

  

## Acknowledgements
- OpenCV  
- face_recognition library  

## License
This project is for educational purposes.
