# Explainable Federated ECG Arrhythmia Classification

An explainable federated learning based ECG arrhythmia classification system developed using FastAPI, TensorFlow/Keras, React, Vite, and Explainable AI techniques.

## Overview

Explainable Federated ECG Arrhythmia Classification is a machine learning based healthcare application for classifying ECG heartbeat signals into different arrhythmia classes. The system uses a trained Federated Averaging model to predict ECG arrhythmia categories from 1D ECG signal samples.

The backend is developed using FastAPI and TensorFlow. It loads the trained federated learning model, receives ECG signal input, performs preprocessing, predicts the arrhythmia class, and provides explainability using saliency and Integrated Gradients methods.

The frontend is developed using React and Vite. It provides a simple user interface where users can generate or paste ECG signal data, visualize the ECG waveform, predict the arrhythmia class, and highlight important ECG regions using Explainable AI.

## Features

* ECG arrhythmia classification
* Federated learning based trained model
* 1D ECG signal input support
* ECG waveform visualization
* Explainable AI support
* Important ECG region highlighting
* Real-time Prediction & Visualization

## Arrhythmia Classes

The model predicts the following ECG heartbeat classes:

* Normal Beat — `N`
* Left Bundle Branch Block Beat — `L`
* Right Bundle Branch Block Beat — `R`
* Atrial Premature Beat — `A`
* Ventricular Premature Beat — `V`

## Technologies Used

### Backend
* Python
* FastAPI
* TensorFlow / Keras
* NumPy

### Frontend
* React
* JavaScript
* Chart Visualization

## Machine Learning Model

This project uses a trained federated learning model for ECG arrhythmia classification.

The deployed model file is:

```text id="1k7yaz"
fedavg_model.h5
```

## Explainable AI

The explanation methods include:

* Saliency Map
* Integrated Gradients

## Dataset

MIT-BIH Arrhythmia Database (PhysioNet)

## Project Structure

```text id="rz1zpf"
Explainable-Federated-ECG-Arrhythmia-Classification-main/
│
├── Backend/
│   ├── xai.py                         # FastAPI backend for prediction and explainability
│   ├── fedavg_model.h5                # Trained Federated Averaging ECG classification model
│   ├── test_x.npy                     # ECG test signal data
│   ├── test_y.npy                     # ECG test labels
│   └── requirements.txt               # Backend dependencies
│
├── Frontend/
│   └── ecg-frontend/
│       ├── public/                    # Public frontend assets
│       ├── src/
│       │   ├── App.jsx                # Main React application
│       │   ├── App.css                # Main frontend styling
│       │   ├── index.css              # Global CSS styling
│       │   ├── main.jsx               # React entry point
│       │   └── assets/                # Frontend assets
│       ├── index.html                 # Main HTML file
│       ├── package.json               # Frontend dependencies and scripts
│       ├── vite.config.js             # Vite configuration
│       └── README.md                  # Default Vite README
│
├── mitbih_database/                   # Dataset
│
└── README.md                          # Project documentation
```

## Learning Purpose

Through this project, the following concepts were practiced:

* Arrhythmia detection
* Federated learning model deployment
* Explainable AI using Saliency Maps & Integrated Gradients
* ECG waveform visualization
* Full-stack machine learning web application development

## License

This project is open-source and available for learning, research, and educational purposes.
