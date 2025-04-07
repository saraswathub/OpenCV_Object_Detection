# OpenCV_Object_Detection
OPenCV and Edge Computing using YOLO11

# YOLO11 on Raspberry Pi: Edge Object Detection

This repository demonstrates how to run the powerful YOLO11 object detection model from Ultralytics on a Raspberry Pi, leveraging on-device inference for low-cost, high-efficiency computer vision. By eliminating latency and cloud costs, this project aims to democratize AI, empowering small businesses, research teams, and hobbyists to build intelligent systems with minimal resources.

In an era where edge computing is becoming the norm, solutions like this represent a leap toward ubiquitous, intelligent systems—bringing robust object detection to every corner of the world.

## Features
- Real-time object detection and tracking using YOLO11.
- Optimized for resource-constrained devices like the Raspberry Pi.
- No cloud dependency—everything runs locally.
- Easy-to-use codebase with essential libraries.

## Why On-Device Inference?
- **Low Latency**: No round-trips to the cloud mean faster results.
- **Cost-Effective**: Avoid hefty cloud fees and scale with minimal hardware.
- **Accessibility**: Empower innovation for teams with tight budgets.

## Prerequisites
- Raspberry Pi (4 upwards recommended for better performance).
- Python 3.7+ installed.
- A camera module (e.g., Raspberry Pi Camera) or USB webcam.
- Basic familiarity with Python and terminal commands.

## Essential Libraries
- **OpenCV (`cv2`)**: Handles video frames, draws bounding boxes, and displays results.
- **NumPy (`np`)**: Manages numerical operations and array handling.
- **`time`**: Measures loop duration for FPS calculation.
- **YOLO (Ultralytics)**: The core deep learning model for detection and tracking.
- **`defaultdict` (collections)**: Simplifies storing tracking data without manual key checks.

## Usage
1. **Download YOLO11 Weights**:
   - Pre-trained weights are available from the [Ultralytics YOLO repository](https://github.com/ultralytics/ultralytics). Place them in the `weights/` folder.

2. **Run the Detection Script**:
   ```bash
   python3 detect.py --source 0  # Use 0 for webcam, or specify a video file path## Customize Parameters (optional)
3. Edit `detect.py` to adjust confidence thresholds, input sources, or display options.

## Example Output
- Video feed with bounding boxes around detected objects.
- Real-time FPS displayed for performance monitoring.

## Performance Tips
- Use a Raspberry Pi 4 with 4GB or 8GB RAM for smoother performance.
- Lower the input resolution (e.g., 320x320) to boost FPS on resource-constrained devices.
- Consider using a lightweight YOLO11 model variant (e.g., YOLO11n) for faster inference.

## Contributing
Contributions are welcome! Feel free to open issues or submit pull requests to improve the codebase or add new features.
