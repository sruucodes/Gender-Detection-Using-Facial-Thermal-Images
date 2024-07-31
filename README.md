# Gender Detection Using Facial Thermal Images

## Overview

This project utilizes deep learning models to detect gender from facial thermal images. The repository includes pre-trained models such as ResNet-50, DenseNet-121, and ResNet-101, which are trained on standard datasets to achieve high accuracy and efficiency in gender detection tasks.

## Table of Contents

- [Overview](#overview)
- [Deep Learning Models](#deep-learning-models)
  - [ResNet-50](#resnet-50)
  - [DenseNet-121](#densenet-121)
  - [ResNet-101](#resnet-101)
- [Datasets Used](#datasets-used)
- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)
- [Contributing](#contributing)

## Deep Learning Models

This repository contains pre-trained deep learning models for gender detection using facial thermal images. The models include:

### ResNet-50

ResNet-50 is a 50-layer residual network developed by Kaiming He et al. It is known for its efficiency and accuracy in various image recognition tasks.

- **File**: [ResNet-50.pt](https://drive.google.com/drive/folders/14usN0kr70S5mBn4r-o5tMsyxWsuYCewC)
- **Parameters**: 23.5 million

### DenseNet-121

DenseNet-121 is a densely connected convolutional network developed by Gao Huang et al. It improves information flow between layers and is known for achieving high accuracy with fewer parameters.

- **File**: [DenseNet-121.pt](https://drive.google.com/drive/folders/14usN0kr70S5mBn4r-o5tMsyxWsuYCewC)
- **Parameters**: 8 million

### ResNet-101

ResNet-101 is a deeper variant of the ResNet architecture, with 101 layers. It provides improved performance on complex image recognition tasks.

- **File**: [ResNet-101.pt](https://drive.google.com/drive/folders/14usN0kr70S5mBn4r-o5tMsyxWsuYCewC)
- **Parameters**: 44.6 million

## Datasets Used

To download the complete datasets, please use the following link:
[Datasets Download Link](https://drive.google.com/open?id=1wGDNfCQE1kngsmYiKlKHHZwgntlVwiGJ)

## Installation

### Prerequisites

Ensure you have the following installed:

- Python 3.8+
- pip

### Setup

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/gender-detection-thermal-images.git
    cd gender-detection-thermal-images
    ```

2. **Create and activate a virtual environment** (optional but recommended):
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install the required dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **If the `requirements.txt` file doesn't exist, manually install the dependencies**:
    ```bash
    pip install torch torchvision
    pip install torchsummary
    pip install numpy matplotlib
    pip install pillow
    ```

## Usage

### Running Pre-trained Models

To run and check the results of each of the pre-trained models, use the `Pretrained_models_testing.ipynb` script in the notebook.

### Running the Testing Script

Run the `testing.ipynb` file to see the output.

```bash
jupyter notebook testing.ipynb
