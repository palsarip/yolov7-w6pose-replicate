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

#### Option 1: Using Anaconda (Recommended)

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

#### Option 2: Using Python venv (Without Anaconda)

1. Clone the repository:

   ```
   git clone https://github.com/yourusername/fallsafei-server-app.git
   cd fallsafei-server-app
   ```

2. Create a virtual environment:

   ```
   python -m venv venv
   ```

3. Activate the virtual environment:

   - On Windows:
     ```
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```
     source venv/bin/activate
     ```

4. Install required packages:

   ```
   # Computer vision dependencies
   pip install opencv-python
   pip install torch torchvision
   pip install matplotlib
   pip install ultralytics
   pip install scikit-image

   # API and backend dependencies
   pip install fastapi>=0.68.0
   pip install uvicorn>=0.15.0
   pip install sqlalchemy
   pip install alembic
   pip install pydantic
   pip install python-dotenv
   pip install psycopg2-binary
   pip install pydantic-settings
   ```

Note: Some packages might have complex dependencies and could be more difficult to install with pip alone compared to Anaconda, especially on Windows systems.

## Project Structure

```
yolov7-w6pose-replicate/
├── datasets/              # Dataset storage
├── models/                # Model weights
├── results/               # Generated outputs
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
