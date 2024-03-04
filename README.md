# Virtual_Mouse

Requirements:
Python 3.x
OpenCV (pip install opencv-python)
MediaPipe (pip install mediapipe)
PyAutoGUI (pip install pyautogui)
Screen Brightness Control (pip install screen_brightness_control)
pycaw (pip install pycaw)
ctypes (pip install ctypes)


Description:
The hand gesture controller program uses a webcam to detect hand gestures and performs various actions based on the recognized gestures. It utilizes the MediaPipe library for hand tracking and gesture recognition, OpenCV for video capture and processing, PyAutoGUI for controlling the mouse and keyboard, screen_brightness_control for adjusting screen brightness, and pycaw for adjusting system volume.

How it Works:
Initialization: The program initializes the necessary libraries and sets up the webcam for capturing video frames.

Hand Detection: Using the MediaPipe library, the program detects the landmarks (key points) on the hand, such as fingertips, knuckles, and palm.

Gesture Recognition: It maps the hand landmarks to specific gestures, such as a closed fist, thumbs up, or a peace sign, using a custom HandRecog class. This class converts the hand landmarks into recognizable gestures.

Action Execution: Based on the recognized gestures, the program performs various actions. For example, it moves the mouse cursor, clicks the mouse buttons, scrolls the screen, adjusts the system volume, or changes the screen brightness.

User Interaction: The program displays the video feed from the webcam with overlaid hand landmarks and gesture annotations. It also listens for user input to exit the program.

Continuous Operation: The program runs in a loop, continuously capturing video frames, detecting hand gestures, and performing actions based on the recognized gestures, providing real-time interaction with the computer.

Usage:
Ensure all required libraries are installed (opencv-python, mediapipe, pyautogui, screen_brightness_control, pycaw, ctypes).
Run the program and follow the on-screen instructions to interact with the computer using hand gestures.
Notes:
The program may require calibration and adjustment of parameters based on the lighting conditions and hand movements for optimal performance.
Use caution when using the program, as it can perform actions that may affect the computer's settings and operations.
