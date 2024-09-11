# Object Detection with YOLOv8 - Self-Driving Cars

## Project Overview
This Jupyter Notebook facilitates object detection tasks for self-driving cars using the YOLOv8 model. It involves environment setup, data handling, and preparation for model training and evaluation.

## Architecture Diagram

![image](https://github.com/user-attachments/assets/9275f1e8-d335-4590-b101-de7ebe09e99a)

The architecture diagram illustrates the following components:
- **Feature Extractor**: This component takes an input image and extracts relevant features using a pre-trained backbone network.
- **Neck**: This intermediate part processes the extracted features and prepares them for the detection head. It typically involves upsampling and concatenation operations.
- **Detection Head**: This final component predicts bounding boxes and class probabilities for the detected objects. It often uses a feature pyramid network (FPN) to handle objects of different sizes.

## Contents
- **Environment Setup**: Ensures the system has the required GPU resources available for training.
- **Data Exploration**: Lists and verifies the contents of the dataset directory, specifically targeting images and labels required for object detection.
- **Directory Configuration**: Creates necessary directories for storing model outputs and other related files.

## Prerequisites
- **Python**: Ensure you have Python 3.x installed.
- **Jupyter Notebook**: This project is designed to be run in a Jupyter Notebook environment.
- **YOLOv8**: Ensure that YOLOv8 is installed and available within your environment.
- **CUDA**: Required for GPU acceleration.

## How to Run
1. **Clone the Repository**: 
   ```
   git clone <repository-url>
   cd <repository-folder>
   ```
2. **Launch Jupyter Notebook**:
   ```
   jupyter notebook Self_driving_vehicles.ipynb
   ```
3. **Execute the Cells**: Follow the sequence of cells in the notebook, starting with environment checks, data loading, and subsequent training processes.

## Dataset
The dataset used in this project should be placed in the `/kaggle/input/self-driving-cars` directory, containing images and corresponding label files in CSV format.

## Outputs
- **Trained Model**: YOLOv8 model files will be saved in the `/kaggle/working/yolov8` directory.
- **Logs and Metrics**: Output from training, including logs and performance metrics, will be stored within the notebook.

## Testing
Here are few images after running our trained model on test images
![image](https://github.com/user-attachments/assets/deb7e95c-df87-4191-b2bb-0c064b1d3cf9)

## Results
![image](https://github.com/user-attachments/assets/b2aa966d-be80-4fd4-ae8d-03feb2770395)

## Acknowledgements
- **YOLOv8**: For the object detection model.
- **Kaggle**: For providing the dataset and computational resources.
