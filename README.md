[![GitHub issues](https://img.shields.io/github/issues/GabrieleAraujo/comparative-optimizer-deeplearning)](https://github.com/GabrieleAraujo/comparative-optimizer-deeplearning/issues) 
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-yellow.svg?style=flat-square)](https://github.com/GabrieleAraujo/comparative-optimizer-deeplearning/pulls) 
[![HitCount](https://views.whatilearened.today/views/github/GabrieleAraujo/comparative-optimizer-deeplearning.svg)](https://github.com/GabrieleAraujo/comparative-optimizer-deeplearning) 
[![website coderjojo.github.io](https://img.shields.io/website-up-down-yellow-red/http/coderjojo.github.io/creative-profile-readme.svg)](GabrieleAraujo)



# Comparative Optimizer Analysis in Deep Learning Tasks

This repository contains the code, data, and analysis used in the paper **"Análise Comparativa de Otimizadores em Tarefas de Classificação e Regressão Utilizando Redes Neurais Profundas"**. The study evaluates different optimizers' performance in classification and regression deep learning tasks using Multi-Layer Perceptrons (MLPs).

## Overview

The goal of this research is to compare the performance of four optimizers—SGD with momentum, Adagrad, RMSprop, and Adam—across two tasks:
- **Sentiment Classification** using the [IMDB movie reviews dataset](https://bit.ly/3BXLvZm).
- **Temperature Regression** using [Belém, Pará, Brazil meteorological data](https://bit.ly/48qC54D).

Key findings from the paper:
- RMSprop demonstrated superior performance in the sentiment classification task (Accuracy: 0.8847).
- SGD with momentum achieved the best results in the regression task (MAE: 0.3973).

## Repository Structure

```bash
Comparative-Optimizer-Analysis-DeepLearning/
├── data/                   # Datasets used in the experiments
│   ├── BrazilWeather     # Dataset for sentiment classification
│   ├── IMDBDataset     # Dataset for temperature regression
├── results/                # Output results, metrics, and figures
│   ├── classification/     # Classification task results
│   ├── regression/         # Regression task results
├── train_classification.py  # Script to train a classification model
├── train_regression.py      # Script to train a regression model
└── README.md               # This file
```

## Results

### Classification Task
For the IMDB sentiment classification, the following results were achieved:

| Model | Optimizer | Accuracy           | F1-Score           |
|-------|-----------|--------------------|--------------------|
| MLP1  | Adam      | 0.8760 ± 0.0138    | 0.8734 ± 0.0192    |
| MLP2  | RMSprop   | 0.8847 ± 0.0073    | 0.8827 ± 0.0105    |
| MLP3  | Adam      | 0.8670 ± 0.0189    | 0.8718 ± 0.0132    |

RMSprop achieved the best overall performance, with an accuracy of **88.47%** and an F1-score of **88.27%**. Adam also performed well across various models.

### Regression Task
For temperature regression using meteorological data, the results were as follows:

| Model | Optimizer          | MAE                |
|-------|--------------------|--------------------|
| MLP1  | SGD with momentum  | 0.3973 ± 0.0549    |
| MLP2  | SGD with momentum  | 0.4140 ± 0.0669    |
| MLP3  | Adam               | 0.4914 ± 0.1511    |

SGD with momentum showed the lowest Mean Absolute Error (MAE) of **0.3973** in the simplest model (MLP1).

Full results are available in the `/results` folder.

## License
This project is licensed under the MIT License.
