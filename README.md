# Hand Gesture Controlled Drawing Application

This application uses a webcam to track hand movements and allows users to draw on a digital canvas using hand gestures. The application is built with OpenCV, MediaPipe, and NumPy, and supports drawing in different colors, changing brush thickness, and drawing shapes like rectangles, circles, and lines.

## Requirements

Before running the application, ensure you have the following installed:

- Python 3.7+
- OpenCV
- MediaPipe
- NumPy

## Installation

1. **Python**: Make sure you have Python installed on your system. You can download it from [python.org](https://www.python.org/downloads/).

2. **Virtual Environment (optional but recommended)**: It's a good practice to create a virtual environment to manage dependencies.
    ```sh
    python -m venv myenv
    source myenv/bin/activate
    ```

3. **Install dependencies**:
    ```sh
    pip install opencv-python mediapipe numpy
    ```

## Usage

1. **Run the application**:
    ```sh
    python aircanvas3.ipynb
    ```

2. **Controls**:
    - `q`: Quit the application
    - `u`: Increase brush thickness
    - `d`: Decrease brush thickness
    - `e`: Eraser mode
    - `r`: Draw rectangle
    - `c`: Draw circle
    - `l`: Draw line
    - `f`: Free draw

3. **Gesture Commands**:
    - **Clear the canvas**: Hover your index finger over the "CLEAR" button.
    - **Change color**: Hover your index finger over the color buttons (BLUE, GREEN, RED, YELLOW).
    - **Draw**: Use your index finger to draw on the canvas. For shapes, move your index finger to define the shape size.

## Code Overview

- **Color Points Storage**: Separate deques for each color to store drawing points.
- **Brush and Shape Settings**: Variables for managing brush thickness and shape modes.
- **UI Setup**: Initial setup for the canvas and UI buttons.
- **Mediapipe Initialization**: Setup for hand tracking using MediaPipe.
- **Webcam Capture**: Loop to capture frames from the webcam and process hand landmarks.
- **Gesture Processing**: Logic to handle drawing, shape creation, and UI interactions based on hand positions.
- **Shape Drawing**: Drawing stored shapes and points on the canvas and frame.

## Example Output

The application displays two windows:
- **Output**: Real-time webcam feed with hand landmarks and drawing.
- **Paint**: The drawing canvas showing the final drawing.

## Troubleshooting

- Ensure your webcam is properly connected and functioning.
- Make sure all dependencies are installed correctly.
- If the hand landmarks are not detected, try adjusting the lighting conditions.

## Contributing

If you'd like to contribute to the project, feel free to submit a pull request or report issues on the GitHub repository.

## License

This project is open-source and available under the MIT License.



---

