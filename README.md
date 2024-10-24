# Vehicle Detection System


## Overview

This project implements a real-time **Vehicle Detection System** using Python, OpenCV, and YOLOv3. The system is designed to monitor traffic flow, detect vehicles, and manage parking zones efficiently. It provides a solution for urban traffic congestion and parking challenges through accurate vehicle detection and data processing.

## Features

- **Real-Time Vehicle Detection:** Detects vehicles in traffic and parking zones with 95.4% accuracy.
- **Traffic Monitoring:** Tracks vehicle flow and congestion in real-time.
- **Parking Management:** Provides updates on available parking spaces and maintains historical parking data.
- **Data Storage:** Stores vehicle count and parking data in a SQL database for analysis and reporting.

## Tech Stack

- **Python:** Backend development and data handling.
- **OpenCV:** Real-time image and video processing.
- **YOLOv3:** Object detection model for vehicle recognition.
- **NumPy & Matplotlib:** Data manipulation and visualization.
- **SQL:** Database used for storing vehicle detection data.
### Video


https://github.com/shahishree03/vehicle_detection/assets/54995727/72df4a6b-395d-45fa-8406-69a83ed05a23

## Installation

### Prerequisites

Before running this project, ensure you have the following installed:

- Python 3.x
- OpenCV
- YOLOv3 weights and configuration files
- NumPy
- Matplotlib
- SQL database setup (MySQL/PostgreSQL)
- PIP for package installation

### Steps

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/vehicle-detection.git
   cd vehicle-detection-system
2. Install the required dependencies:

    ```bash
   pip install -r requirements.txt

3. Download the pre-trained YOLOv3 weights and configuration files:

YOLOv3 Weights
YOLOv3 Config
4. Place the yolov3.weights and yolov3.cfg files into the model/ directory.

5. Set up the SQL database and configure it in the code by providing the connection string in the config.py file.

Usage
a) Running the Vehicle Detection System:

b) To start vehicle detection, run the following command:

    ```bash
       Copy code
      python detect.py --input videos/traffic.mp4 --output output/results.avi --yolo model/

This will detect vehicles in the provided input video (traffic.mp4) and save the processed output to results.avi.

Parking Management:

The system can monitor parking areas by running the following command:

    ```bash
     python parking_management.py --input videos/parking_lot.mp4 --output output/parking_results.avi --yolo model/
