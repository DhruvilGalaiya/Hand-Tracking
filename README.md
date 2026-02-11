# Hand-Tracking
A computer vision application that allows users to control their system volume using hand gestures (pinching) via a webcam, built with Python, OpenCV, and MediaPipe.

# Volume Hand Control 🔊👆

This project uses computer vision to control your computer's system volume with hand gestures. It detects your hand using a webcam and calculates the distance between your thumb and index finger to adjust the volume level.

## How It Works
- **Detection**: Uses MediaPipe to detect hand landmarks [1].
- **Interaction**: Calculates the distance between the thumb (tip 4) and index finger (tip 8) [3], [4].
- **Feedback**: A volume bar and percentage are displayed on the screen [5]. The center button turns green when the volume is "clicked" (fingers pinched) [6].

## Prerequisites
To run this project, you need to install the following libraries [7], [8]:
* opencv-python
* mediapipe
* pycaw
* numpy

## How to Run
1. Ensure `HandTrackingModule.py` is in the same folder as the main script [2].
2. Run the main volume control script.
3. Bring your hand in front of the camera.
4. Pinch your thumb and index finger to change the volume.

## Credits
* Inspired by Murtaza's Workshop - Robotics and AI [1].
* Volume control library (pycaw) by Andre Miras [8].
