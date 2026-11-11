# Emotion Detection from Text

A Flask web application that predicts an emotion label from text using saved model and preprocessing artifacts.

## Repository layout

    app.py                   Flask application entry point
    templates/index.html     Web interface
    preprocess.ipynb         Preprocessing and model workflow
    emotion_model.pkl        Trained classifier
    vectorizer.pkl           Text vectorizer
    label_encoder.pkl        Label mapping
    train.txt                Training examples
    val.txt                  Validation examples
    test.txt                 Test examples
    render.yaml              Deployment configuration

## Run locally

Prerequisites: Python and pip.

Create an isolated environment and install the pinned dependencies:

    python -m venv .venv
Windows PowerShell:

    .venv\Scripts\Activate.ps1

macOS or Linux:

    source .venv/bin/activate
    python -m pip install -r requirements.txt

Start the application:

    python app.py

Open the local address printed by Flask.

## Model files

The model, vectorizer, and label encoder are used together by the application. Keep them in the repository root unless the loading paths in app.py are deliberately updated.

## Notes

The requirements file contains a broad pinned environment. The notebook records the preprocessing workflow; the tracked artifacts are the model used by the web application.
