# Object Detection with YOLO

This repository contains code for object detection using the YOLO (You Only Look Once) algorithm. It utilizes the OpenCV library for real-time object detection in videos.

## Features

- Detects objects in input videos or real-time webcam feed.
- Uses a pre-trained YOLO model on the COCO dataset for object detection.
- Provides options to adjust confidence threshold and non-maxima suppression threshold.
- Outputs annotated videos with detected objects.

## Usage

### Prerequisites

- Python 3.x
- OpenCV library (`pip install opencv-python`)

### Running the Code

1. Clone the repository:

    ```bash
    git clone https://github.com/ARCHANAREDDY15/your-repo.git
    ```

2. Navigate to the repository directory:

    ```bash
    cd your-repo
    ```

3. Run the script `optimised.py` with the following command:

    ```bash
    python optimised.py --input path/to/input/video.mp4 --output path/to/output/video.avi --yolo path/to/yolo/coco
    ```

    Replace `path/to/input/video.mp4` with the path to your input video file, `path/to/output/video.avi` with the desired path for the output video, and `path/to/yolo/coco` with the path to the YOLO directory containing the configuration file and weights.

4. View the annotated output video to see the detected objects.

## Intel oneAPI Usage and Analysis

This project can be further optimized for performance using Intel oneAPI tools and libraries. By leveraging Intel's hardware acceleration capabilities, such as Intel Integrated Graphics and Intel CPUs, you can achieve faster inference speeds and improved efficiency.

### Prerequisites

- Intel oneAPI Base Toolkit (Install from [here](https://software.intel.com/content/www/us/en/develop/tools/oneapi/base-toolkit/download.html))
- Intel Distribution of OpenVINO toolkit (Optional)

### Optimizing with Intel oneAPI

1. Install the Intel oneAPI Base Toolkit and Intel Distribution of OpenVINO toolkit (if desired).

2. Use the Intel oneAPI tools, such as Intel VTune Profiler, to analyze the performance bottlenecks in the code and identify areas for optimization.

3. Utilize Intel oneAPI libraries, such as oneDNN (Deep Neural Network Library) and oneVPL (Video Processing Library), to accelerate inference and video processing tasks.

4. Implement optimizations, such as parallelization, vectorization, and offloading to accelerators, using Intel oneAPI programming models like DPC++ and OpenMP.

5. Measure the performance improvements achieved by the optimizations and compare them with the baseline implementation.

## Example Output

### Input Video
<img src="car_chase_01.mp4">


### Output Video
[![Output Video](https://example.com/output_video_thumbnail.png)](path/to/output/video.avi)
