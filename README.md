# ForestSmokeDetection

ForestSmokeDetection is a project for detecting smoke in forest environments. The goal is to fine-tune an object detection model (RT-DETR) to quickly identify the presence of smoke in forest images. This project is part of an effort to improve environmental monitoring and early warning systems.

## Table of Contents

- [Description](#description)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)

Description

This project aims to develop a system that automatically detects smoke in forest images. By fine-tuning an object detection model, we strive to create an efficient tool for monitoring forest areas and providing early alerts in case of smoke detection.

## Project Structure
```plaintext
ForestSmokeDetection/
├── README.md                   
├── .gitignore                  
├── requirements.txt            
├── dataset/            
│   ├── images/
│   │   ├── train/              
│   │   └── val/                
│   ├── labels/
│   │   ├── train/              
│   │   └── val/                
│   └── data.yaml               
├── notebooks/
│   ├── Data_Import_and_Training.ipynb   
│   └── Inference_Evaluation.ipynb        
├── src/                        
└── SmokeDetectEnv/             
---

Prerequisites
- Python 3.8 or higher
- Git
- A virtual environment manager 

---

Installation
Cloning the Repository
Clone the repository to your local machine using the following command:


'git clone https://github.com/VictorPro07/ForestSmokeDetection.git'
'cd ForestSmokeDetection'

Creating and Activating a Virtual Environment

Using venv:

'python -m venv SomkeDetectEnv'
'source SomkeDetectEnv/bin/activate'   # On Linux/MacOS


Installing Dependencies
Install the required Python packages with:

'pip install -r requirements.txt'


Usage

Model Training
Open the Data_Import_and_Training.ipynb notebook using VSCode, Jupyter Notebook, or JupyterLab.
Ensure that the dataset/data.yaml file correctly points to your image and annotation directories.
Execute the cells in the notebook to start training the model and also to import the dataset.


Inference and Evaluation
Open the Inference_Evaluation.ipynb notebook.
This notebook allows you to test the trained model on new images and evaluate its performance.
Follow the instructions within the notebook to run inference and visualize the results.

Dataset Configuration
The dataset/data.yaml file contains the dataset configuration, including:
train: Path to the training images.
val: Path to the validation images.
labels: Paths to the training and validation annotations.
names: A list of classes (e.g., 0: smoke).
nc: The number of classes (in this case, 1).
Make sure these paths correctly reflect the structure of your dataset.

