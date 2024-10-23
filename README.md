# Comparative Optimizer Analysis in Deep Learning Tasks

This repository contains the code, data, and analysis used in the paper **"Análise Comparativa de Otimizadores em Tarefas de Classificação e Regressão Utilizando Redes Neurais Profundas"** by *Gabriele S. Araújo* and *Omar A. Carmona Cortes*. The study evaluates different optimizers' performance in classification and regression deep learning tasks using Multi-Layer Perceptrons (MLPs).

## Overview

The goal of this research is to compare the performance of four optimizers—SGD with momentum, Adagrad, RMSprop, and Adam—across two tasks:
- **Sentiment Classification** using the IMDB movie reviews dataset.
- **Temperature Regression** using Belém, Pará, Brazil meteorological data.

Key findings from the paper:
- RMSprop demonstrated superior performance in the sentiment classification task (Accuracy: 0.8847).
- SGD with momentum achieved the best results in the regression task (MAE: 0.3973).

## Repository Structure

```bash
Comparative-Optimizer-Analysis-DeepLearning/
├── data/                   # Datasets used in the experiments
│   ├── BrazilWeather     # Dataset for sentiment classification
│   ├── IMDBDataset     # Dataset for temperature regression
├── train_classification.py  # Script to train a classification model
├── train_regression.py      # Script to train a regression model
├── results/                # Output results, metrics, and figures
│   ├── classification/     # Classification task results
│   ├── regression/         # Regression task results
└── README.md               # This file
