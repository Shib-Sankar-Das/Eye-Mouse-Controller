# 👀 Eye-Mouse-Controller 🖱️ 

Welcome to the **Eye-Controlled Mouse** project! This project leverages computer vision and machine learning to create a hands-free mouse control system powered by eye and facial landmarks. Using your webcam, this system detects and tracks eye movements, translating them into mouse actions such as movement, left-click, and right-click. It's a unique way to control your computer—just with your eyes! 🖱️

---

## 🧠 Project Approach

This project combines several tools to achieve eye-tracking mouse control:
1. **OpenCV**: Captures real-time video from your webcam.
2. **MediaPipe**: Tracks facial landmarks, particularly focusing on eye regions.
3. **PyAutoGUI**: Controls the mouse based on the processed eye movement data.

### Step-by-Step Process:
1. **Face Detection and Landmark Extraction**: Uses MediaPipe's FaceMesh model to identify and refine facial landmarks.
2. **Eye Region Identification**: Tracks specific landmark points around the eyes to detect gaze direction and eye closure.
3. **Mouse Movement**: Maps eye positions to the screen’s coordinates.
4. **Click Detection**: Uses the distance between key eye landmarks to determine blinking, allowing left and right-click actions.

---

## 💡 Key Features

- **Hands-Free Control**: Move the mouse cursor with your eye movements, left-click by blinking, and right-click with a specific eye gesture.
- **Real-Time Processing**: Uses a webcam feed, giving quick and responsive cursor control.
- **Enhanced Accessibility**: Ideal for users with mobility limitations, providing an alternative interaction method with computers.

---

## 🔧 Installation

### Requirements
- **Python 3.7+**
- **OpenCV**
- **MediaPipe**
- **PyAutoGUI**

### Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/Shib-Sankar-Das/Eye-Controlled-Mouse.git

2. Install the required packages:
  ```bash
    pip install opencv-python mediapipe pyautogui
  ```

3. Run the project:
  ```bash
    python EyeMouseController.py
