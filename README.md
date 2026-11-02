# ML Streamlit App

A simple machine-learning web application that predicts an Iris flower species from four measurements using a Random Forest classifier.

## Features

- Interactive Streamlit interface for entering flower measurements
- Iris species prediction: Setosa, Versicolor, or Virginica
- Pre-trained model loaded locally with Joblib
- Training script to regenerate the model

## Project structure

```text
ML_Streamlit_App/
├── app.py             # Streamlit user interface
├── train.py           # Trains and saves the classifier
├── iris_model.pkl     # Saved Random Forest model
├── iris.csv           # Iris dataset file
└── requirements.txt   # Python dependencies
```

## Requirements

- Python 3.9 or newer
- pip

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Negesh44/ML_Streamlit_App.git
   cd ML_Streamlit_App
   ```

2. Create and activate a virtual environment (recommended):

   ```bash
   python -m venv .venv
   .venv\Scripts\activate
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Run the app

Start the Streamlit application:

```bash
streamlit run app.py
```

Open the local URL displayed in your terminal, usually `http://localhost:8501`.

## Train the model

The repository includes a saved model. To retrain it from scikit-learn's Iris dataset, run:

```bash
python train.py
```

This creates or replaces `iris_model.pkl`, which the application uses for predictions.

## Inputs

Enter measurements in centimetres for:

- Sepal length
- Sepal width
- Petal length
- Petal width

Click **Predict** to see the predicted species.

## Tech stack

- Python
- Streamlit
- scikit-learn
- Joblib

## License

This project is available for learning and personal use.
