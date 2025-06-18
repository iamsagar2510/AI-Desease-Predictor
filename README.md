# AI Disease Predictor

A web-based AI tool for predicting possible diseases based on patient health parameters using machine learning. Built with [Streamlit](https://streamlit.io/), [scikit-learn](https://scikit-learn.org/), and [Plotly](https://plotly.com/python/).

## Features

- Predicts disease based on user input (age, gender, BMI, BP, sugar, cholesterol, smoking status, family history)
- Shows prediction confidence and top 3 probable diseases
- Provides health recommendations
- Interactive and modern UI



## Getting Started

### Prerequisites

- Python 3.8 or higher (Python 3.10/3.11 recommended)
- pip

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/iamsagar2510/AI-Desease-Predictor.git
   cd AI-Desease-Predictor
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Make sure you have the following files in the project folder:**
   - `app.py` (the Streamlit app)
   - `model.pkl` (your trained ML model)
   - `health_data.csv` (your original training data)

### Running the App

```bash
streamlit run app.py
```
If you get a "command not found" error, use the full path to `streamlit.exe` or add it to your PATH.

The app will open in your browser at [http://localhost:8501](http://localhost:8501).

## Project Structure

```
.
├── app.py
├── model.pkl
├── health_data.csv
├── requirements.txt
└── README.md
```

## How It Works

- The app loads your training data and fits label encoders for categorical features.
- User inputs are encoded and passed to the trained model for prediction.
- The app displays the predicted disease, confidence, and health tips.

## Customization

- To use your own data/model, replace `health_data.csv` and `model.pkl` with your files.
- Update the input fields in `app.py` if your features are different.

## License

This project is for educational purposes.

---

**Made with ❤️ by Sagar Das