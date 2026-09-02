# Deepfake Detection

This repository contains the source code and selected results used in the engineering thesis:

**"Wykrywanie obrazów typu deepfake z wykorzystaniem konwolucyjnych sieci neuronowych"**

The project focuses on detecting deepfake images using two convolutional neural network architectures:

- SimpleCNN, a convolutional neural network implemented from scratch in PyTorch
- ResNet50, a pretrained model using transfer learning

## Dataset

The experiments were conducted using the **Deepfake and Real Images** dataset available on Kaggle:

https://www.kaggle.com/datasets/manjilkarki/deepfake-and-real-images/data

The dataset is divided into training, validation and test sets. The images are resized to 224 × 224 pixels and converted to tensors before being passed to the models.

The dataset itself is not included in this repository.

## Repository structure

- `code/` contains the source code used for data preparation, model training and evaluation
- `figures/` contains figures generated during the experiments
- `results/` contains selected results of the experiments
- `README.md` contains the project description
- `.gitignore` contains files excluded from version control

## Models

### SimpleCNN

A convolutional neural network implemented from scratch using PyTorch. The architecture consists of three convolutional blocks followed by fully connected layers.

### ResNet50

A pretrained ResNet50 model with ImageNet weights. Transfer learning was used by adapting the final classification layer and partially fine tuning the network.

## Requirements

The project requires Python and the following main libraries:

- PyTorch
- torchvision
- NumPy
- scikit-learn
- Matplotlib
- PIL

## Author

Zuzanna Jaroszczyk
