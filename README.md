# computervision_motionfiltering_opencv

# Motion Detection using OpenCV

This is a basic computer vision script that detects motion in a CCTV-style video using OpenCV's MOG2 background subtraction.

## Overview

The script processes a video (`humans_walking_cctv.mp4`) and uses OpenCV's `createBackgroundSubtractorMOG2` to isolate moving objects—typically humans walking—against a static background.

The mask (binary foreground image) is displayed in real time, and the script loops the video when it reaches the end.

## How It Works

- Opens the video file using `cv.VideoCapture`
- Applies a background subtractor (`MOG2`) to each frame
- Displays the foreground mask
- Repeats video when it ends
- Stops when you press the `x` key

## Dependencies

- Python 3.x
- OpenCV (cv2)

Install OpenCV:

pip install opencv-python
