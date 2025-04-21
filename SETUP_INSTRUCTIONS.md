# Emotion-based Music Recommendation System - Setup Instructions

This project analyzes your facial expressions using your webcam, identifies your emotional state, and recommends music that matches your mood.

## System Requirements

- Python 3.7-3.11 (TensorFlow does not support Python 3.12+ as of 2024)
- Webcam
- Windows, macOS, or Linux

## Installation Steps

1. **Create a Python virtual environment with a compatible Python version**

   This project requires Python 3.7-3.11 due to TensorFlow compatibility constraints.

   ```bash
   # Install a compatible Python version if needed
   # Then create a virtual environment
   python -m venv venv

   # Activate the virtual environment
   # On Windows:
   venv\Scripts\activate
   # On macOS/Linux:
   source venv/bin/activate
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application**

   ```bash
   streamlit run app.py
   ```

## Troubleshooting

- **TensorFlow installation issues**: If you're having problems installing TensorFlow, try installing specific versions:
  ```bash
  pip install tensorflow==2.10.0
  ```

- **OpenCV camera access**: Make sure your webcam is not in use by another application and that you've granted necessary permissions.

- **Model loading errors**: Ensure all file paths in app.py correctly point to the model files.

## Usage

1. Click the "SCAN EMOTION" button
2. The app will use your webcam to capture images of your face
3. Your emotion will be analyzed in real-time
4. Based on your emotional state, the system will recommend songs
5. Click on any recommended song to visit its web page

## Project Structure

- `app.py`: Main application code
- `model.h5`: Pre-trained emotion detection model
- `haarcascade_frontalface_default.xml`: Face detection cascade classifier
- `muse_v3.csv`: Music dataset with emotional tags
- `requirements.txt`: Required Python packages

## License

This project is based on the work of [Hiral Sathwara](https://github.com/Hiralsathwara/Emotion-based-music-recommendation-system) 