# Computer Vision Hand-Tracking
A computer vision application that allows users to control their system volume using hand gestures (pinching) via a webcam, built with Python, OpenCV, and MediaPipe.

# Volume Controller 🔊👁️

An interactive Computer Vision application that allows you to control your system volume using hand gestures. By pinching your thumb and index finger, you can adjust the volume in real-time.

## 📂 Project Structure (File Guide)

Here is what each file in this project does:

*   **`VolumeControl.py` (Main File)**: 
    *   **Run this file.** This is the main application script. 
    *   It turns on your webcam, runs the main loop, calculates the distance between your fingers, and draws the volume bar on the screen [1-3].
    
*   **`HandTrackingModule.py` (Helper Module)**: 
    *   **Do not run this directly.** This is a backend helper file.
    *   It contains the logic to detect hands and find specific landmarks (like finger tips). The main file imports this module to make the code cleaner and easier to read [4, 5].
    *   *Note: Keep this file in the same folder as `VolumeControl.py` or the project will not work.*

## 🚀 Key Features
*   **Computer Vision**: Uses OpenCV and MediaPipe to track hand movements without special hardware.
*   **Real-time Interaction**: Adjusts volume instantly based on finger distance [6].
*   **Visual Feedback**: Displays a dynamic volume bar and percentage on the screen [7, 8].

## 🛠️ How to Run
1.  Install the required libraries:
    ```bash
    pip install opencv-python mediapipe pycaw numpy
    ```
2.  Make sure `VolumeControl.py` and `HandTrackingModule.py` are in the same folder.
3.  Run the main file:
    ```bash
    python VolumeControl.py
    ```
## Important Note ##
Make sure to run this project on python version "3.9".
