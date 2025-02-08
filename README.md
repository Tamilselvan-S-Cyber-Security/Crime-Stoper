# Setting Up a Virtual Environment with Anaconda

## 1. Install Anaconda
Download and install Anaconda from:  
[Anaconda Official Download](https://www.anaconda.com/download)

---

## 2. Create a Virtual Environment
Open **Anaconda Prompt** or **Terminal** and run:

```bash
conda create --name dlib_env
  ```
## 3. Activate the Virtual Environment
Run the following command:

## Windows:
```bash
conda activate dlib_env
  ```

   ```bash
pip install streamlit opencv-python-headless ultralytics numpy pandas pygame pyttsx3 torch Pillow
 ```

## 2. Install Dependencies from requirements.txt
Run the following command to install all the packages listed in the file:
 ```bash
pip install -r requirements.txt
 ```
## 3. Run the application:
   ```bash
   streamlit run app.py
   ```

## Usage Guide

1. **Starting the System**:
   - Launch the application using `streamlit run app.py`
   - Select your preferred camera source from the dropdown menu

2. **Configuring Detection**:
   - Adjust the confidence threshold using the slider
   - Set the target object name (default: "person")
   - Upload custom target images for specific detection
   - Monitor the live feed and detection statistics

3. **Custom Target Detection**:
   - Click "Upload Target Image" in the sidebar
   - Select a PNG or JPEG image of your target
   - The system will automatically compare detected objects with your target

4. **Managing Alerts**:
   - Automatic audio and visual alerts when objects are detected
   - Voice announcements of detected objects
   - Export detection data using the "Export Detection Data" button

5. **Viewing Results**:
   - Real-time camera feed with detection boxes

## Future Features

- Multi-camera support for simultaneous monitoring
- Night vision enhancement for low-light conditions
- Facial recognition integration
- Advanced motion tracking
- Custom alert configurations
- Enhanced target matching algorithms

## Project Structure

```
├── app.py              # Main application file
├── utils/
│   ├── alert.py       # Alert system implementation
│   ├── detection.py   # Object detection utilities
│   └── logger.py      # Logging functionality
├── data/              # Detection logs and data
├── targets/           # Custom target images
└── detections/        # Saved detection images


# Project Title

## Demo Video 🎥  
<video width="600" controls autoplay loop muted>
  <source src="https://fit-ai-english.web.app" type="video/mp4">
  Your browser does not support the video tag.
</video>
