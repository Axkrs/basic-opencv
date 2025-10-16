md
# basic-opencv

This project demonstrates basic face detection using OpenCV (cv2) in Python. It captures video from a webcam, converts each frame to grayscale, and uses a Haar Cascade classifier to detect faces, drawing rectangles around them.

## Key Features & Benefits

*   **Real-time Face Detection:** Detects faces in real-time video stream from a webcam.
*   **Simple Implementation:** Provides a clear and concise example of using OpenCV for face detection.
*   **Educational Resource:**  Serves as a good starting point for learning about computer vision and OpenCV.

## Prerequisites & Dependencies

Before running this project, you need to have the following installed:

*   **Python:**  Version 3.6 or higher is recommended.
*   **OpenCV (cv2):** Install using pip: `pip install opencv-python`
*   **NumPy (optional):** OpenCV usually depends on NumPy, but you might need to install it explicitly: `pip install numpy`

## Installation & Setup Instructions

1.  **Clone the Repository:**

    ```bash
    git clone https://github.com/Axkrs/basic-opencv.git
    cd basic-opencv
    ```

2.  **Install Dependencies:** (If you haven't already)

    ```bash
    pip install opencv-python
    ```

3.  **Verify Installation:**

    You can quickly verify that OpenCV is installed correctly by running python and importing `cv2`:

    ```python
    import cv2
    print(cv2.__version__)
    ```

## Usage Examples

To run the face detection script:

1.  **Navigate to the project directory:**

    ```bash
    cd basic-opencv
    ```

2.  **Execute the `facetrack.py` script:**

    ```bash
    python facetrack.py
    ```

    This will open a window displaying the webcam feed with rectangles around detected faces.

3.  **Exit:** Press `q` in the video window to close the application.

## Configuration Options

The following parameters can be adjusted within the `facetrack.py` script to customize the face detection:

*   **`scaleFactor`:** In `face_cascade.detectMultiScale()`. This parameter specifies how much the image size is reduced at each image scale.  A smaller value increases detection accuracy but also increases computation time.  Default value: 1.1.

*   **`minNeighbors`:**  In `face_cascade.detectMultiScale()`. This parameter specifies how many neighbors each candidate rectangle should have to retain it. A higher value results in fewer detections but decreases false positives. Default value: 5.

*   **`cv2.VideoCapture(0)`:**  Change the camera index if you have multiple webcams. `0` typically refers to the default webcam.  Try `1`, `2`, etc. if the default camera is not used.

## Contributing Guidelines

Contributions are welcome! Here are the general guidelines:

1.  Fork the repository.
2.  Create a new branch for your feature or bug fix.
3.  Make your changes and ensure they are well-tested.
4.  Submit a pull request with a clear description of your changes.

## License Information

This project has no specified license. All rights are reserved by the owner, Axkrs.

## Acknowledgments

*   OpenCV (cv2): For providing the computer vision library used for face detection.
