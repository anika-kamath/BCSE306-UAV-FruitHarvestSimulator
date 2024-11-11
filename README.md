# BCSE306-UAV-FruitHarvestSimulator

## Overview

The project utilizes a customized CoppeliaSim scene featuring a quadcopter that follows a defined trajectory while using Vision RGB sensors to hover over an orchard. The sensor feed is processed through a VGG16 neural network, along with custom color masking for yellow and orange hues, to detect the presence of ripe mangoes in the orchard for harvesting purposes.

## Software Used

- Quadcopter and Environment Modelling and Simulation: CoppeliaSim
- Custom architecture and RGB Spectral Masking: Jupyter Notebook (Python)

## Features

- Custom Path Planning for Quadcopter using Trajectory Definition
- Reading sensor feeds and converting it into frames for further processing
- Color masking and VGG 16 processing to detect ripe mangoes in the orchard simulation.

## Prerequisites

- Python 3.x installed on your machine.
- GPU support for faster processing (recommended).
- NVIDIA GPU with CUDA support.
- CoppeliaSim Edu Installed.

## Installation

1. Clone this repository to your local machine:
   ```
   git clone https://github.com/anika-kamath/BCSE306-UAV-FruitHarvestSimulator.git
   ```

2. Run the CoppeliaSim Scene to observe the trajectory:
   ```
   run the .ttt file
   ```

3. Verify the processing of the model using the ipynb file:

## Usage

1. Ensure you have access to a GPU. You can use the `!nvidia-smi` command to check GPU availability.
   
2. Download the pre-trained YOLOv8 model:
   ```
   !gdown 'pre-trained-model-url'
   ```

3. Load the pre-trained YOLOv8 model and set up the Supervision library.

4. Run the provided scripts to detect and track vehicles in videos:
   ```
   python vehicle_detection_tracking.py
   ```
