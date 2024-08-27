### Weather-image-classification-using-YOLO

# Project Overview
This project is designed to classify weather conditions in images using the YOLOv8 (You Only Look Once, Version 8) model. YOLOv8 is a state-of-the-art object detection model known for its speed and accuracy. In this project, we train YOLOv8 to recognize various weather conditions, such as sunny, cloudy, rainy, and snowy, within images.

# Table of Contents
Project Overview
Installation
Dataset
Training
Inference
Evaluation
Results
Contributing
License
Acknowledgments
Installation
To run this project, you need to set up your environment with the required dependencies. Follow the steps below to get started:
Clone the repository:
git clone https://github.com/yourusername/weather-image-classification-yolov8.git
cd weather-image-classification-yolov8

Install dependencies:

Make sure you have Python 3.8 or later installed. Then, install the required packages:
pip install -r requirements.txt

Set up YOLOv8:

If YOLOv8 is not included in requirements.txt, you can install it using:
pip install ultralytics

Dataset
The dataset used for training the model consists of images categorized into various weather conditions. If you have a custom dataset, ensure it is organized in the following structure:

dataset/
├── images/
│   ├── train/
│   │   ├── sunny/
│   │   ├── cloudy/
│   │   ├── rainy/
│   │   ├── snowy/
│   ├── val/
│   │   ├── sunny/
│   │   ├── cloudy/
│   │   ├── rainy/
│   │   ├── snowy/
├── labels/
│   ├── train/
│   │   ├── sunny/
│   │   ├── cloudy/
│   │   ├── rainy/
│   │   ├── snowy/
│   ├── val/
│   │   ├── sunny/
│   │   ├── cloudy/
│   │   ├── rainy/
│   │   ├── snowy/

Download the dataset and place it in the dataset/ directory.

# Training
To train the YOLOv8 model on your dataset:

Configure the training settings:

Edit the config.yaml file to set your dataset paths, hyperparameters, and other configurations.

Run the training script:
python train.py --config config.yaml

This will start training the model and save the best weights to the runs/ directory.

# Acknowledgments
Special thanks to the YOLOv8 development team for providing an excellent object detection framework.
This project was inspired by various weather classification tasks in computer vision.
