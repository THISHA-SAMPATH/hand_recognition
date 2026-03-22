# Hand Recognition — Streamlit App

Real-time hand detection using OpenCV and Streamlit. 
Uses HSV skin color segmentation to detect and isolate 
hands from a live webcam feed.

## How it works
- Captures webcam feed using OpenCV
- Converts frames to HSV color space
- Applies skin color mask (HSV range: 0-20, 20-255, 70-255)
- Uses morphological operations + Gaussian blur to clean the mask
- Displays the isolated hand region in real time via Streamlit

## Run locally
```bash
pip install -r requirements.txt
streamlit run hand_recognition/app.py
```

## Tech Stack
Python · Streamlit · OpenCV · NumPy
