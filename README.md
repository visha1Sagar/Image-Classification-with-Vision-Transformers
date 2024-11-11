# Satellite Image Classification with Vision Transformers

This project leverages Vision Transformers to classify satellite images, aiding in monitoring deforestation in the Amazon. The model classifies various features in satellite images, which can help policymakers and local stakeholders respond quickly to environmental changes.

## Project Overview
Deforestation in the Amazon is a critical issue, leading to biodiversity loss, habitat destruction, and climate change. This project analyzes satellite images to detect signs of deforestation and human encroachment, using machine learning to classify and monitor forest health from space.

## Features
- **Data Import**: Downloads and loads Amazon's Planet dataset of satellite images.
- **Data Preprocessing**: Normalizes, resizes, and encodes satellite image data.
- **Model**: Implements a Vision Transformer model to detect features such as cloud cover, water, agriculture, and other land cover types.
- **Training & Evaluation**: Includes data augmentation and splitting for robust model training and evaluation.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/visha1Sagar/Image-Classification-with-Vision-Transformers.git
   cd Image-Classification-with-Vision-Transformers
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Running the Notebook
1. Open `Analyzing_Amazon_Using_Vision_Transformer.ipynb` and run each cell to execute data loading, training, and evaluation.

2. Key settings include:
   - Image size: 64x64 pixels
   - Patch size for Transformer: 8x8 pixels
   - Training parameters: 35 epochs, batch size of 128

## Model Architecture
### Vision Transformer (ViT)
A custom Vision Transformer (ViT) is built with the following specifications:
- **Layers**: 5 Transformer layers with 4 attention heads
- **Embedding Size**: 64-dimensional patch embeddings
- **MLP Head**: Fully connected layers for classification


## Performance
### Losses
![image](https://github.com/user-attachments/assets/990163d4-9a8d-4ec1-b78d-5dcdab9ff394)
### F-Beta Scores
![image](https://github.com/user-attachments/assets/a0986ff4-ded0-4331-969d-4b287cbb27b8)


## Acknowledgments
Dataset by Planet, accessible on Kaggle. This project also utilizes libraries such as TensorFlow, Keras, OpenCV, and Matplotlib.
