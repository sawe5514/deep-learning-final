# Final Project: Image Captioning

## 1. Problem Description

### 1.1 Project Goal
The goal of this project is to build a deep learning model that can automatically generate a descriptive text caption for a given image. This is a fascinating multimodal problem that combines techniques from both Computer Vision and Natural Language Processing (NLP).

### 1.2 Model Architecture: An Encoder-Decoder Approach
To solve this, we will implement an **encoder-decoder** model, a common architecture for this type of task.
- **Encoder:** We will use a pretrained Convolutional Neural Network (CNN), specifically VGG16, to process the input image. The CNN will act as a feature extractor, converting the raw image pixels into a rich vector representation that captures the key objects and scenes in the image. This leverages the power of transfer learning.
- **Decoder:** We will use a Recurrent Neural Network (RNN), specifically an LSTM (Long Short Term Memory) network, to generate the caption. The LSTM will take the feature vector from the encoder as its initial input and generate the caption one word at a time, learning the structure and vocabulary of natural language.

### 1.3 Data Source
The dataset used is the Flickr8k dataset, which contains 8,000 images, each paired with five different human generated captions.
- **Source:** [Kaggle: Flickr 8k Dataset](https://www.kaggle.com/datasets/adityajn105/flickr8k)
