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
```
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
1.Sample Output of a Male image
![image](https://github.com/user-attachments/assets/101fb7cb-588b-4b41-884f-0401ef4462b8)
The DenseNet model successfully analyzed the infrared image and predicted the gender as Male. Infrared images, by capturing thermal patterns, offer unique features that DenseNet can effectively utilize for such tasks.


2.Sample Output of a Female Image
(![image](https://github.com/user-attachments/assets/5ba66be4-6a54-4ea5-bc97-507bde55b5cd)
The ResNet-50 model successfully analyzed the infrared image and predicted the gender as Female. Infrared images, by capturing thermal patterns, offer unique features that ResNet-50 can effectively utilize for such tasks

3.  Misclassified Female as Male
![image](https://github.com/user-attachments/assets/eafc3402-7dc6-49c2-8bfc-fcac85a80188)

The ResNet-50 model failed to analyze the infrared image and predicted the gender as Male, which was truly a Female. Infrared images, by capturing thermal patterns, offer unique features that ResNet-50 can effectively utilize for such tasks


CONFUSION MATRICES
1.  Confusion Matrix for DenseNet-121
 ![image](https://github.com/user-attachments/assets/d1f416cf-d834-455a-810a-a6341dfa6743)

The DenseNet-121 confusion matrix reveals that the model correctly classified 51 males and 26 females. However, it misclassified 4 males as females and 9 females as males. This indicates that while DenseNet-121 is quite accurate, it has a higher rate of false negatives, meaning it sometimes fails to identify females correctly.

2.  Confusion Matrix for ResNet-50
![image](https://github.com/user-attachments/assets/a44c84a6-f048-467b-82a6-cc87981da15b)

The ResNet-50 confusion matrix indicates that the model effectively distinguishes between males and females, correctly classifying 51 males and 30 females. The model's performance is highlighted by its lower misclassification rates, with only 4 males incorrectly identified as females and 5 females misclassified as males.

3. Confusion Matrix for ResNet-101
![image](https://github.com/user-attachments/assets/7c19ba66-2b97-471c-a05c-f0c50c4dc694)

The ResNet-101 confusion matrix demonstrates that the model effectively identifies males, correctly classifying 54 out of the total. However, it shows more difficulty with female classification, correctly identifying only 21 females while misclassifying 14 females as males.


## Contributing
1. Sahithi Srujana C
2. Pinni Sruthi Raga
3. Rakshith V Patil
4. Raunak Singh Rathour
