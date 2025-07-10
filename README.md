# CompDinoBarlow Project

## Overview

The **CompDinoBarlow** project focuses on implementing and evaluating self-supervised learning techniques using the Barlow Twins architecture with ResNet-18 and ResNet-50 backbones. The project includes training, testing, and visualization of metrics for EuroSAT dataset classification tasks.

## Project Structure

- `training_Res18.ipynb`: Notebook for training the ResNet-18 backbone with the Barlow Twins method.
- `training_Res50.ipynb`: Notebook for training the ResNet-50 backbone with the Barlow Twins method.
- `testing_Res18.ipynb`: Notebook for linear probing and evaluating the trained ResNet-18 model on the EuroSAT dataset.
- `testing_Res50.ipynb`: Notebook for linear probing and evaluating the trained ResNet-50 model on the EuroSAT dataset.
- `models/`: Directory containing the trained model checkpoints.

## Features

- **Training**: Self-supervised learning using Barlow Twins architecture with ResNet-18 and ResNet-50 backbones.
- **Testing**: Linear probing for classification tasks on the EuroSAT dataset.
- **Visualization**: Metrics such as confusion matrices and t-SNE plots for feature embeddings.
- **Augmentation**: Advanced data augmentation techniques for robust training.

## Requirements

- Python 3.8+
- PyTorch
- torchvision
- h5py
- tqdm
- scikit-learn
- seaborn
- matplotlib
- TensorBoard

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/hamze258/CompDinoBarlow.git
   cd CompDinoBarlow
   ```

2. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

1.  **Training**: Open and run the `training_Res18.ipynb` or `training_Res50.ipynb` notebook to train the corresponding model.
2.  **Testing**: After training, open and run the `testing_Res18.ipynb` or `testing_Res50.ipynb` notebook to evaluate the model and generate visualizations.

## Results

The project demonstrates the effectiveness of the Barlow Twins method for self-supervised learning on the EuroSAT dataset. The ResNet-50 model achieves a higher accuracy compared to the ResNet-18 model, as expected. The t-SNE plots show a clear separation of classes, indicating that the learned features are highly discriminative.

## Visualizations

- **Confusion Matrix**: Visualizes the performance of the classification model.
- **t-SNE Plot**: Shows the 2D projection of the high-dimensional feature embeddings, illustrating the separability of the learned classes.
- **Collage**: A random collage of 20 images with their predicted and true labels.