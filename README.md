# Emotion Detection from Text

A Flask web application that predicts an emotion label from text using saved model and preprocessing artifacts.

## Repository layout

    app.py                  Flask application entry point
    templates/              Web interface
    models/                 Classifier, vectorizer, and label encoder
    data/                   Training, validation, and test examples
    notebooks/              Preprocessing and model-training notebooks
    requirements.txt        Python dependencies

## Run locally

Prerequisites: Python and pip.

Create an isolated environment and install the pinned dependencies.

Windows PowerShell:

    python -m venv .venv
    .venv\Scripts\Activate.ps1

macOS or Linux:

    python -m venv .venv
    source .venv/bin/activate

Install dependencies and start the application:

    python -m pip install -r requirements.txt
    python app.py

Open the local address printed by Flask.

## Model files

The model, vectorizer, and label encoder are loaded from models/ and used together by the application. Keep them paired with the preprocessing workflow that produced them.

## Data handling

The text files in data/ are used for model development. Avoid committing private or personally identifiable data.
