# MLP vs CNN: Architecture, Efficiency and Inductive Bias

This project investigates how Multi-Layer Perceptrons and Convolutional Neural Networks perform across image-classification tasks of different complexity.

The models are implemented and evaluated using PyTorch on the MNIST and CIFAR-10 datasets. The project explores how architecture, parameter count, computational efficiency and inductive bias influence model performance and generalisation.

## Project Objectives

The project compares MLP and CNN architectures across two datasets:

* **MNIST**, consisting of grayscale handwritten digit images
* **CIFAR-10**, consisting of colour images from ten object classes

The experiments investigate:

* the effect of increasing model complexity
* differences between fully connected and convolutional architectures
* training and validation performance
* parameter efficiency
* computational cost
* generalisation across simple and complex visual datasets
* the effect of convolutional inductive bias

## Methods

The project includes:

* reproducible dataset preprocessing
* training, validation and test splits
* dataset-specific normalisation
* reusable PyTorch training and evaluation functions
* MLP and CNN architecture implementations
* parameter-count analysis
* training-time measurement
* hyperparameter experiments
* training and validation curve analysis
* efficiency and generalisation comparisons

## Repository Structure

```text
mlp-vs-cnn-comparison/
├── notebook/
│   └── mlp-vs-cnn-comparison.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Technologies

* Python
* PyTorch
* torchvision
* NumPy
* pandas
* Matplotlib

## Datasets

The project uses the MNIST and CIFAR-10 datasets provided through `torchvision.datasets`.

The datasets are downloaded automatically when the notebook is run and are therefore not included in this repository.

## Running the Project

1. Clone this repository.

2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

3. Open the notebook:

```text
notebook/mlp-vs-cnn-comparison.ipynb
```

4. Run the notebook cells in order.

The datasets will be downloaded automatically when required.

## Key Analysis

The experiments compare MLP and CNN performance across datasets with different visual complexity.

The project examines why MLPs can perform well on relatively simple image data such as MNIST, while CNNs generally provide stronger parameter efficiency and generalisation on spatially complex image data such as CIFAR-10.

The analysis also considers the role of convolutional inductive bias, including local connectivity, shared weights and spatial feature extraction.
