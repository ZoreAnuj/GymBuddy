# GymBuddy - Your Personal Trainer with Pose Detection

This Python script uses the trt pose library and OpenCV to detect and track human pose from a webcam feed. It can be used as a foundation for various applications, including personal fitness training, yoga posture detection, or even just as a fun tool to learn more about computer vision.

trt_pose: https://github.com/NVIDIA-AI-IOT/trt_pose

## Table of Contents

1. [Installation](#1-installation)
2. [Basic Usage](#2-basic-usage)
3. [Pose Detection](#3-pose-detection)
4. [Calculating Angles](#4-calculating-angles)
5. [Curl Counter](#5-curl-counter)

## 1. Installation

Before using this script, you need to install the required dependencies. You can do this by running the following command:

```bash
!pip install opencv-python
```

## 2. Basic Usage

The script captures video from your webcam, detects the human pose, and visualizes it on the screen. You can stop the script by pressing 'q' while the video feed window is active.

## 3. Pose Detection
The script uses the MediaPipe library to detect and track the human pose. It uses the following landmarks to identify the body's position:

Left Shoulder
Left Elbow
Left Wrist
These landmarks help in calculating the angle of the arm during specific exercises or poses.

## 4. Calculating Angles
The calculate_angle function in the script calculates the angle between three points (shoulder, elbow, and wrist). It is used to measure the angle of the arm during exercises or poses.

## 5. Curl Counter
The script includes a curl counter feature that counts how many times a specific motion is performed. It counts the number of curls based on the angle of the arm and changes in position. The current count and stage (up or down) are displayed on the screen.

Feel free to modify and build upon this script to create your own personal trainer or fitness-tracking applications!

Enjoy using GymBuddy :)
