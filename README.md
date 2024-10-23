# Comparative Optimizer Analysis in Deep Learning Tasks

This repository contains the code, data, and analysis used in the paper **"Análise Comparativa de Otimizadores em Tarefas de Classificação e Regressão Utilizando Redes Neurais Profundas"** by *Gabriele S. Araújo* and *Omar A. Carmona Cortes*. The study evaluates the performance of different optimizers in deep learning tasks of classification and regression using Multi-Layer Perceptrons (MLPs).

## Overview

The goal of this research is to compare the performance of four optimizers—SGD with momentum, Adagrad, RMSprop, and Adam—across two tasks:
- **Sentiment Classification** using the IMDB movie reviews dataset.
- **Temperature Regression** using meteorological data from Belém, Pará, Brazil.

Key findings from the paper:
- RMSprop demonstrated superior performance in the sentiment classification task (Accuracy: 0.8847).
- SGD with momentum achieved the best results in the regression task (MAE: 0.3973).

## Repository Structure

```bash
Comparative-Optimizer-Analysis-DeepLearning/
├── data/                   # Datasets used in the experiments
│   ├── imdb_dataset.csv     # Dataset for sentiment classification
│   ├── weather_data.csv     # Dataset for temperature regression
├── models/                 # Pre-trained models or saved checkpoints
├── scripts/                # Python scripts for training and evaluation
│   ├── train_classification.py  # Script to train classification model
│   ├── train_regression.py      # Script to train regression model
├── results/                # Output results, metrics, and figures
│   ├── classification/     # Classification task results
│   ├── regression/         # Regression task results
└── README.md               # This file
