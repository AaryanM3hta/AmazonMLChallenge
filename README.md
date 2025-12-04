Amazon ML Challenge 2025

Attempted the Amazon ML Challenge. The challenge won — but I learned a lot anyway.

Project Overview

This repository contains my submission for the Amazon ML Challenge 2025.
I worked as part of Team Codo-sapiens (Aaryan Mehta) and built a multimodal regression model that uses both text and image information to predict product prices.

The idea was straightforward:

Use a BERT-based model to understand product descriptions

Use CLIP to understand product images

Combine both embeddings

Train a neural network to estimate the final price

Even though I didn’t qualify further, this project was a great learning experience in multimodal machine learning, embeddings, and model design.

Methodology
1. Text Embedding Generation

Notebook: AML-NLPtrain.ipynb

Cleans and preprocesses product text

Generates sentence embeddings using a SentenceTransformer (BERT-based) model

Saves the embeddings for later use

2. Image Embedding Generation

Notebook: CNNmodel_CLIP.ipynb

Downloads product images

Uses the CLIP vision model to extract image embeddings

Saves the embeddings for the final model

3. Final Regression Model

Notebook: Regression_model.ipynb

Loads both text and image embeddings

Concatenates them into a multimodal feature vector

Trains an ANN regressor

Generates the final submission.csv file
## **License**
This project is licensed under the Apache 2.0 License. See the `LICENSE` file for details.
