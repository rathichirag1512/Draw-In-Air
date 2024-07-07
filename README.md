# Air Draw 

Ever wished to capture your imagination by just waving your finger in the air? In this project, we have an Air Canvas that can draw anything on it by simply moving our hands and observing the landmark on the hand knuckles. A virtual drawing tool (Computer vision project) that allows you to draw in the air using hand gestures, thanks to the powerful combination of OpenCV and MediaPipe.

## 🔧 Tools and Libraries Used

- Python3
- NumPy
- OpenCV
- MediaPipe

## OpenCV

This open-source library is essential for real-time computer vision tasks. It helps capture and process video frames from the webcam seamlessly.

## MediaPipe

Developed by Google, MediaPipe is a fantastic framework for building multimodal machine learning pipelines. In this project, MediaPipe is used for hand tracking, enabling accurate and real-time recognition of hand landmarks.

## How It Works

1. **Capture Video**: Using OpenCV, the script captures live video feed from the webcam.
2. **Process Frames**: Each frame is processed using MediaPipe to detect and track hand landmarks.
3. **Draw Landmarks**: The detected hand landmarks are drawn on the video frames, creating a virtual canvas for drawing in the air.

## Algorithm

1. Start reading the frames and convert the captured frames to HSV colour space (easy for colour detection).
2. Prepare the canvas frame and put the respective ink buttons on it.
3. Adjust the values of the MediaPipe utilization to detect one hand only.
4. Detect the landmarks by passing the RGB frame to the MediaPipe hand detector.
5. Detect the landmarks, find the forefinger coordinates, and keep storing them in the array for successive frames (arrays for drawing points on canvas).
6. Finally, draw the points stored in an array on the frames and canvas.

