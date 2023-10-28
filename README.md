# Image Caption Generation on COCO_5070 Dataset

Automatically generate descriptive captions for images using the COCO_5070 dataset, and evaluate the model using BLEU scores and cosine similarity.

## Table of Contents
- [Introduction](#introduction)
- [Data Preparation](#data-preparation)
- [Feature Extraction](#feature-extraction)
- [RNN-based Decoder Training](#rnn-based-decoder-training)
- [Caption Generation & Evaluation](#caption-generation--evaluation)
- [Metrics Comparison](#metrics-comparison)
- [Conclusion](#conclusion)
- [Getting Started](#getting-started)
- [Acknowledgments](#acknowledgments)

## Introduction
This project aims to design and evaluate an image captioning model that can automatically produce descriptive captions for images. The model's performance is assessed using two metrics: BLEU score and cosine similarity.

## Data Preparation
- Loaded the COCO_5070 dataset comprising images and their associated captions.
- Cleaned captions: converted them to lowercase, eliminated punctuations, and added start and end tokens.
- Constructed a vocabulary from the dataset's unique words.
- Split the dataset into training, validation, and test sets.

## Feature Extraction
- Utilized a pre-trained ResNet-50 model as an encoder to obtain features from images.
- Extracted a fixed-size feature vector from each image using the final fully connected layer of ResNet-50.

## RNN-based Decoder Training
- Designed the DecoderRNN model that ingests the image features and produces captions.
- Monitored training and validation losses over several epochs to train the model.

## Caption Generation & Evaluation
- Used the trained model to derive captions for the test images.
- Evaluated the quality of the generated captions against the reference captions using BLEU scores.
- Assessed the semantic similarity of the generated captions to the reference captions using cosine similarity.

## Metrics Comparison
- Analyzed and contrasted the results procured from BLEU scores and cosine similarity.
- Delved into individual examples to comprehend scenarios where the metrics aligned and where they diverged.

## Conclusion
Successfully designed, trained, and assessed an image captioning model. The BLEU score and cosine similarity metrics provided comprehensive insights into the model's capability to generate pertinent and descriptive captions for images.


## Acknowledgments
- COCO dataset creators and maintainers.
- ResNet-50 authors and contributors.
- OpenAI and the community for research and resources.

