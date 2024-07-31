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

- **File**: [`ResNet-50.pt`](https://drive.google.com/drive/folders/14usN0kr70S5mBn4r-o5tMsyxWsuYCewC)
- **Parameters**: 23.5 million

### DenseNet-121

DenseNet-121 is a densely connected convolutional network developed by Gao Huang et al. It improves information flow between layers and is known for achieving high accuracy with fewer parameters.

- **File**: [`DenseNet-121.pt`](https://drive.google.com/drive/folders/14usN0kr70S5mBn4r-o5tMsyxWsuYCewC)
- **Parameters**: 8 million

### ResNet-101

ResNet-101 is a deeper variant of the ResNet architecture, with 101 layers. It provides improved performance on complex image recognition tasks.

- **File**: [`ResNet-101.pt`](https://drive.google.com/drive/folders/14usN0kr70S5mBn4r-o5tMsyxWsuYCewC)
- **Parameters**: 44.6 million

## Datasets Used

To download the complete datasets, please use the following link:
[Datasets Download Link](https://drive.google.com/open?id=1wGDNfCQE1kngsmYiKlKHHZwgntlVwiGJ)

## Installation

⁠ bash
    pip install torch torchvision
    pip install torchsummary
    pip install numpy matplotlib
    pip install pillow
     ⁠


### Prerequisites

Ensure you have the following installed:

- Python 3.8+
- pip

### Setup

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/gender-detection-thermal-images.git
    cd gender-detection-thermal-images
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

### Running Pre-trained Models

To run and check the results of each of the pre-trained models, use the `Pretrained_models_testing.ipynb` script in the notebook.

### Running the Testing Script

Run the `testing.ipynb` file to see the output.

```bash
jupyter notebook testing.ipynb

```
## Examples

SAMPLE OUTPUTS

1. ![image](https://github.com/user-attachments/assets/101fb7cb-588b-4b41-884f-0401ef4462b8)
Sample Output of a Male image

The DenseNet model successfully analyzed the infrared image and predicted the gender as Male. Infrared images, by capturing thermal patterns, offer unique features that DenseNet can effectively utilize for such tasks.

2. ![image](https://github.com/user-attachments/assets/5a318ab0-652d-4009-9898-ebfba01dbb04)
Sample Output of a Female Image

The ResNet-50 model successfully analyzed the infrared image and predicted the gender as Female. Infrared images, by capturing thermal patterns, offer unique features that ResNet-50 can effectively utilize for such tasks


3.![image](https://github.com/user-attachments/assets/7b0196a6-93da-4bf8-bdee-de592efba45a)
 Misclassified Female as Male
 
The ResNet-50 model failed to analyze the infrared image and predicted the gender as Male, which was truly a Female. 

CONFUSION MATRICES

1.![image](https://github.com/user-attachments/assets/49b6ce68-7156-4aa5-9477-2b7c5a9fddfb)


  Confusion Matrix for DenseNet-121

The DenseNet-121 confusion matrix reveals that the model correctly classified 51 males and 26 females. However, it misclassified 4 males as females and 9 females as males. This indicates that while DenseNet-121 is quite accurate, it has a higher rate of false negatives, meaning it sometimes fails to identify females correctly.

2. ![image](https://github.com/user-attachments/assets/a44c84a6-f048-467b-82a6-cc87981da15b)

   
  Confusion Matrix for ResNet-50

The ResNet-50 confusion matrix indicates that the model effectively distinguishes between males and females, correctly classifying 51 males and 30 females. The model's performance is highlighted by its lower misclassification rates, with only 4 males incorrectly identified as females and 5 females misclassified as males.

3. ![image](https://github.com/user-attachments/assets/7c19ba66-2b97-471c-a05c-f0c50c4dc694)


  Confusion Matrix for ResNet-101

The ResNet-101 confusion matrix demonstrates that the model effectively identifies males, correctly classifying 54 out of the total. However, it shows more difficulty with female classification, correctly identifying only 21 females while misclassifying 14 females as males.


## Contributing
1. Sahithi Srujana C
2. Pinni Sruthi Raga
3. Rakshith V Patil
4. Raunak Singh Rathour
