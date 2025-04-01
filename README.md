# YOLOv7 W6pose Replicate (From MDPI Journal)

A computer vision-based system for detecting falls and distinguishing them from normal physical activities like push-ups. This project uses YOLO object detection, pose estimation, and activity recognition to identify potential fall incidents.

<!-- ## Project Overview

This system monitors video feeds to detect people, analyze their body positions and movements, and classify activities. When a fall is detected, the system can provide alerts. The project uses YOLO11 for object detection, OpenCV for image processing, and deep learning for activity recognition.

The system is built with a FastAPI backend, allowing for easy integration with other services and front-end applications.

## Features

- Real-time person detection
- Pose estimation for skeletal tracking
- Activity classification (falls vs. exercise activities)
- Customizable alert thresholds
- Support for camera integration
- RESTful API endpoints for integration with other services
- Database storage for event logging and analysis

## Environment Setup

### Requirements

This project requires Python 3.12 and Anaconda or Miniconda to manage dependencies. -->

### Installation

#### Using Anaconda

1. Clone the repository:

   ```
   git clone https://github.com/yourusername/yolov7-w6pose-replicate.git
   cd yolov7-w6pose-replicate
   ```

2. Create a conda environment:

   ```
   conda create -n cv_env python=3.12
   conda activate cv_env
   ```

3. Install required packages:
   ```
   conda install -c conda-forge opencv
   conda install pytorch torchvision -c pytorch
   conda install -c conda-forge matplotlib
   pip install ultralytics
   ```

## Project Structure

```
yolov7-w6pose-replicate/
├───datasets                # Dataset storage
│   └───FallDataset
│       ├───test
│       │   ├───labels
│       │   └───video
│       ├───train
│       │   ├───labels
│       │   └───video
│       └───valid
│           ├───labels
│           └───video
├───results                # Generated outputs
│   ├───test
│   ├───train
│   └───valid
├── models/                # Model weights
├── paper/                 # Paper reference
├── utils/                 # yolov7 wongkinyiu functionalities
└── README.md              # This file
```

## Usage

1. Activate the environment:

   - If using Anaconda:
     ```
     conda activate cv_env
     ```
   - If using venv:
     - Windows: `venv\Scripts\activate`
     - macOS/Linux: `source venv/bin/activate`

2. Place the videos that you want to train in the datasets folder. Recommended for data splitting are 60% training set, 20% validation set, and 20% test set.

3. Run the yolov7-w6pose.ipynb
