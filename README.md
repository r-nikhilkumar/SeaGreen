# SeaGreen

## Identifying Plastics and Submerged Debris in Water Using YOLOv8, Drone, and Camera

### Overview

The Seagreen Project leverages advanced computer vision techniques to detect plastics and submerged debris in water bodies. By using a drone equipped with a camera, we capture video footage of water surfaces and process the frames using the YOLOv8 (You Only Look Once) object detection model. This project aims to contribute to environmental conservation efforts by identifying and locating water pollution sources.

### Table of Contents

- [Overview](#overview)
- [Algorithm](#algorithm)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Contribution](#contribution)
- [License](#license)

## Algorithm

1. **Frame Capture**:
    - Use a drone equipped with a camera to capture video footage of water surfaces.
2. **Frame Preprocessing**:
    - Convert frames from the video to a format suitable for YOLOv8 processing.
3. **Object Detection**:
    - Apply YOLOv8 to detect plastics and submerged debris in the frames.
4. **Post-processing**:
    - Filter and annotate detected objects for further analysis and reporting.

## Requirements

- Python 3.8+
- NumPy
- OpenCV
- PyTorch
- YOLOv8

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/r-nikhilkumar/SeaGreen.git
    cd seagreen
    ```

2. Create a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required libraries:
    ```bash
    cd ./backend
    pip install -r requirements.txt
    cd ../frontend
    npm i
    ```

## Usage

1. Run the script:
    ```bash
    cd ../backend
    python manage.py migrate
    cd ../frontend npm start
    ```

2. The script will process the video, detect plastics and submerged debris, and display the results with annotations.

## How It Works

1. **Frame Capture**: The drone captures video footage of water surfaces. Each frame from the video is extracted for processing.

2. **Frame Preprocessing**: Frames are converted to a suitable format (e.g., resizing, normalization) for YOLOv8.

3. **Object Detection**: The YOLOv8 model, pre-trained on relevant datasets, processes each frame to detect objects. Bounding boxes, labels, and confidence scores are generated for plastics and submerged debris.

4. **Post-processing**: Detected objects are filtered based on confidence scores. Annotations are added to the frames, and results are saved or displayed for analysis.

## Contribution

We welcome contributions to the Seagreen Project. To contribute:

1. Fork the repository.
2. Create a new branch: `git checkout -b my-feature-branch`
3. Make your changes and commit them: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-feature-branch`
5. Submit a pull request.

Please ensure your contributions adhere to the existing code style and include appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

By following these steps and guidelines, you can contribute to the Seagreen Project and help in the identification and reduction of water pollution sources.
